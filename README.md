# TAZ4 Firmware und Anpassungen

## Changelog 
## 05.09.2018
* Update Marlin 1.0.0.1 -> 1.1.9
* Kann nun mit der neuen Arduino IDE komiliert werden
* Sicherheitsfunktionen "Thermal Runaway" aktiviert
* Anpassung der neuen 1.1.9 Firmware auf das E3D Hotend mit der 0.4 Düse
* Kleinere Anpassungen für Qualitätsverbesserung

Diese Anpassungen sind für den TAZ4.
Folgende Anpassungen wurden durchgeführt:

* E3D V6 Hotend
* Maximaler Z Vorschub
* Neuere Marlin Version

Zudem wurde am RamBo Board die Verkabelung angepasst.
Hintergrund ist das der Z-Treiber auf über 100°C angestiegen ist und daher keine Bewegung in der Z-Achse mehr möglich war. 

![](https://github.com/fablab-ka/TAZ4/blob/master/IMG_1071.JPG)
![](https://github.com/fablab-ka/TAZ4/blob/master/IMG_1074.JPG)

Voraussetzung für das Kompilieren: 
## Für Marlin 1.1.9
* Arduino IDE 1.8+
* Ultimaker RamBo Libary -> https://raw.githubusercontent.com/ultimachine/ArduinoAddons/master/package_ultimachine_index.json
* U8glib

## Für Marlin 1001
* Arduino IDE 1.6 (neuere bringen einen Fehler)
* Rambo Libarys
* U8glib
Die benötigten Libarys befinden sich im Ordner Arduino. 
Die Ordnerstruktur muss beibehalten werden.


## Verkabelung des Rambo Boards

Damit die Treiber gekühlt werden, muss der Lüfter auf dem Rambo Board umverkabelt werden.
Der neue Slot ist auf dem Board oben links zu finden.
Wichtig ist die Polarität. Rot muss nach oben zeigen.

![](https://github.com/fablab-ka/TAZ4/blob/master/Rambo_-2.jpg)
![](https://github.com/fablab-ka/TAZ4/blob/master/IMG_1075.JPG)
