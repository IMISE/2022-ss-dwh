# Übungen

Hier finden sich Dateien (Werkzeuge und Hilfedokumente) zum Modul [Data Warehouses und Data Repositories für medizinizische Forschung und Versorgung 2022](https://moodle2.uni-leipzig.de/course/view.php?id=36862/), die für die Arbeit während der Übungen benötigt werden.

## Übung 1: Kohortensuche mit i2b2 (S. Stäubert)

## Übung 2: FAIRification medizinischer Daten (M. Löbe)
**Am besten schon *vor der Übung* herunterladen und installieren!**

### Vorbereitung
#### onFHIR-Repository
Die Installation des FHIR-Servers ist optional. Es stehen alternativ Repositories während der Übung zur Auswahl.

- per Skript: https://github.com/fair4health/common-data-model/releases/tag/v1.1.2
- Selbstbau aus GitHub: https://github.com/fair4health/common-data-model/tree/master/docker
- Download von DockerHub (mit Doku): https://hub.docker.com/r/fair4health/onfhir

#### Data Curation Tool (DCT)
- [Data Curation Tool V1.2.5](https://github.com/fair4health/data-curation-tool/releases) für Windows, Linux, MacOS

#### Data Privacy Tool (DPT)
- [Data Privacy Tool  V1.1.1](https://github.com/fair4health/data-privacy-tool/releases) für Windows, Linux, MacOS

### Benutzung

#### Data Curation Tool
FHIR-Repositories zur Auswahl:
- Student 01: http://nisa3zjndxmyk33y.myfritz.net:8201/fhir/metadata
- Student 02: http://nisa3zjndxmyk33y.myfritz.net:8202/fhir/metadata
- Student 03: http://nisa3zjndxmyk33y.myfritz.net:8203/fhir/metadata
- Student 04: http://nisa3zjndxmyk33y.myfritz.net:8204/fhir/metadata
- Student 05: http://nisa3zjndxmyk33y.myfritz.net:8205/fhir/metadata
- Student 06: http://nisa3zjndxmyk33y.myfritz.net:8206/fhir/metadata

Terminologiedienst (optional): https://health-digital-term.ari-health.eu

Dokumentation: [Deliverable 4.1 Annex I - DataCurationTool_UserGuide.pdf](Anleitungen/D4.1-Annex-I_DataCurationTool_UserGuide.pdf)

Youtube: [Demonstration of the FAIR4Health solution in the FAIR4Health Final Assembly](https://www.youtube.com/watch?v=1nwcxeqiwAw) (24.11.2021)

Beispieldatensätze zum Mapping mit dem DCT
- [F4H_Demo](Demodaten/F4H_DEMO.zip): Demodaten aus FAIR4Health (732 Patienten)
- [VHF_DEMO](Demodaten/VHF_DEMO.zip): Demodaten für den 6. Projektathon der MII (1.000 Patienten)

##### Tipps
- *Start* bzw. *Next* sind rechts oben in der GUI, damit kommt man weiter!
- Logfiles befinden sich unter
  - macOS: ~/Library/Logs/FAIR4Health Data Curation Tool/log.txt
  - Windows: %USERPROFILE%\AppData\Roaming\FAIR4Health Data Curation Tool\logs\log.txt
  - Linux: ~/.config/FAIR4Health Data Curation Tool/logs/log.txt

#### Data Privacy Tool

Dokumentation: [Deliverable 4.1 Annex I - DataCurationTool_UserGuide.pdf](Anleitungen/D4.1-Annex-II_DataPrivacyTool_UserGuide.pdf)

Beispieldatensätze (müssen zuvor in ein FHIR-Repository geladen werden, bspw. mit [Postman](https://www.postman.com/))
- [F4H_Demo](Demodaten/F4H_DEMO.zip): Demodaten aus FAIR4Health (in FAIRified Data)
- [VHF_DEMO](Demodaten/VHF_DEMO.zip): Demodaten für den 6. Projektathon der MII (in FAIRified Data)
- [20 Beispielpatienten](Demodaten/20patients.json) als Bundle (16 Frauen, 4 Männer)
- [100 Beispielpatienten](Demodaten/100patients.json) als Bundle (gerade noch übersichtlich)