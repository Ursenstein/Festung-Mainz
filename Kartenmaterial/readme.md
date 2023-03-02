---

title:        Georefrenzierung
date:         2020-10-15
author:       Christian Unger @cunger
licence:      CC BY 4.0 (https://creativecommons.org/licenses/by/4.0/)
contact:      cunger@students.uni-mainz.de
tags:         DMGK, QGIS, Festung, Mainz, Georeferencing

---
# to-do

- [ ] Einfügen der Punkte
- [ ] Link zum Kartenoverview einbauen
- [ ] Tabellen in .md Format transformieren

# Kartenmaterial

Das der Georefrenzierung zugrunde liegende Kartenmaterial ist eine Sammlung aus verschiedenen Archiven.
Die Ausgangskarten befinden sich im Ordner `/Kartenmaterial/Karten_Ausgansmaterial`.
Zunächst wurden alle Karten gesichtet, Inhalt und Bildqualität überprüft und nach "Referenzierbarkeit" geordnet.

In den Tabellen `Sichtung_Kartenmaterial_Gesamtp` & `Sichtung_weitere_Karten` der Datei `/Kartenmaterial/Karten_Overview.ods` befindet sich die durchgeführte Analyse.

# Referenzlayer

Zur Auffindung von Refrerenzpunkten der Historischen Karten wurden meherere Begehungen der Stadt Mainz durchgeführt.
Auffällige Architekturen und Bauwerke, deren Strukturen sich bis in die Zeit der zu refrenzierdenden  Karten erstreckt, wurden in einem Layer festgehalten:
`/QGIS-Referenzpunktelayer/REFERENZLAYER.geojson`

## Bauwerke `REFERENZLAYER.geojson`

- Fort Karl
- Fort Weisenau
- Fort Malakoff
- Blockhaus
- Gustavsburg
- Rheinschanze (Fragmente)
- Fort Alte Mainspitze
- Zitadelle
- Drususstein
- Fort Stahlberg
- Römermauer
- Gautor
- Fort Phillip
- Ravellin Martin
- Bastion Alexander
- Fort Joseph
- Kavalier Hauptstein
- Kavalier Prinz Holstein
- Fort Hartenberg
- Kirche des Karmeliterklosters
- Kirche St. Christoph
- Reichklarakirche
- Kirche St. Peter
- Staatskanzlei/Altes Zeughaus
- Reduit Kastel
- Befestigung auf der Petersaue



Weitere Referenzierung wurde anhand von Ortophotos und *WMS-Services* durchgeführt:

- Luftbild RP Basisdienst: `http://geo4.service24.rlp.de/wms/dop_basis.fcgi?VERSION=1.1.1&`
- Liegenschaftskarte RP Basisdienst: `http://geo4.service24.rlp.de/wms/lika_basis.fcgi?VERSION=1.1.1`
- DOP rgb (Luftbild Hessen; Land Hessen): `https://www.geoportal.hessen.de/mapbender/php/mod_showMetadata.php/../wms.php?layer_id=52123&PHPSESSID=c7ukptv9d00gt2pb8d7jses2k4&VERSION=1.1.1&withChilds=1`
- Liegenschaftskarte Graustufen (Land Hessen): `https://www.geoportal.hessen.de/mapbender/php/mod_showMetadata.php/../wms.php?layer_id=52079&PHPSESSID=c7ukptv9d00gt2pb8d7jses2k4&VERSION=1.1.1&withChilds=1`

# Referenzierung

Die Referenzierung wurde chronologisch, beginnend mit der jüngsten Karte ausgeführt.
Welche Referenzierung dabei auf welcher, bereits vorher Referenzierten Karte beruht ist in der Tabelle `Referenzierung` der Datei `/Kartenmaterial/Karten_Overview.ods` enthalten.

Die bei der Referenzierung gewählten Punkte befindet sich im Ordner `/Kartenmaterial/Karten_Ausgangsmaterial/points/`

Die Georeferenzierten Karten befinden sich im Ordner: `/Kartenmaterial/Georeferenziert/` (**EPSG 25832**)
