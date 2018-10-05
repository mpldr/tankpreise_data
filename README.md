# Intro
Historische Benzinpreisdaten in Deutschland als CSV-Dateien.

# Preise
Im Verzeichnis _prices_ sind alle Preisänderungen aller Tankstellen in jeweils einer CSV-Datei pro Tag protokolliert.
Felder im CSV-Header:
`date,station_uuid,diesel,e5,e10,dieselchange,e5change,e10change`
Bedeutung:
|Feld        |Bedeutung                                      |
|------------|-----------------------------------------------|
|date        |Änderungszeitpunkt                             |
|station_uuid|UUID der Tankstelle aus `stations`             |
|diesel      |Preis Diesel                                   |
|e5          |Preis Super E5                                 |
|e10         |Preis Super E10                                |
|dieselchange|0=keine Änderung, 1=Änderung, 2=Entfernt, 3=Neu|
|e5change    |0=keine Änderung, 1=Änderung, 2=Entfernt, 3=Neu|
|e10change   |0=keine Änderung, 1=Änderung, 2=Entfernt, 3=Neu|


# Tankstellen
Im Verzeichnis _stations_ sind alle Tankstellen in einer CSV-Datei aufgeführt

# Zuordnung
Jede Tankstelle ist eindeutig über eine UUID identifiziert. In den Preisdaten wird diese UUID referenziert.

# Lizenz der Datensammlung
<https://creativecommons.org/licenses/by-nc-sa/4.0/>
Für kommerzielle Nutzung stellen wir die Daten unter anderer Lizenz zur Verfügung. Nachfrage unter <info@tankerkoenig.de>
