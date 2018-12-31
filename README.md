# Open Verein
Wie du deinen Verein gründest und weitere coole und wichtige Infos. Wir freuen uns über [Issues](https://github.com/chaostreff-flensburg/openverein/issues) oder [Pull Requests](https://github.com/chaostreff-flensburg/openverein/pulls) mit Verbesserungen.

Satzung und Beitragsordnung vom [Chaostreff Flensburg e.V.](https://chaostreff-flensburg.de/mitmachen/satzung/)

**Disclaimer:** Wir übernehmen keine Haftung für Richtigkeit des Inhalts, freuen uns aber über Verbesserungen und Tipps!

## Vereinsgründung
### Was wird alles für die Gründung von einem Verein gebraucht
- Sieben Menschen für die Gründungsversammlung ([§ 56 BGB](https://www.gesetze-im-internet.de/bgb/__56.html))
- Satzung / Beitragsordnung
- Sitz und eine Post Anschrift
- Mindestens einen Menschen für die Vorstandsarbeit (üblicherweise aber mindestens 3) ([§ 26 Abs. 1 Satz 2 BGB](https://www.gesetze-im-internet.de/bgb/__26.html))
- Geld für die Eintragung (ca. 130€)
- Ordner für die Bürokratie

```mermaid
graph LR
  start(Finde sieben Menschen) --> founding
  founding(Gründungssitzung) --> gemd
  gemd{Gemeinnützig?} --> |ja| satzcheckf
  gemd --> |nein| amtsgericht
  satzcheckf{Finanzamt: Stzung checken lassen} --> |ja| amtsgericht
  satzcheckf --> |nein| nachbessern
  nachbessern(Nachbessern) --> satzcheckf
  amtsgericht(Amtsgericht)
```
```mermaid
graph LR
  cam2(DESK CAM) -->|HDMI| switch0
  A[Presenter] -->|HDMI| switch0>Switch 0]
  switch0 -->|HDMI| switch1>Switch 1]
  switch1 -->|HDMI| elgato(Elgato)
  hdmiaudiosplit1 -->|HDMI| beamer(Beamer)
  switch1 -->|HDMI| beamer
  cam1(SPEAKER CAM) -->coverter(LINDY Converter)
  funkempf1(Funk-Empfänger 1) -.-|Klinke| soundcard
  funkempf2(Funk-Empfänger 2) -.-|Klinke| soundcard
  switch2-->|HDMI| hdmiaudiosplit1(HDMI/Audio-Splitter)
  soundcard ===|USB| USBHub
  USBHub(Usb Hub) ===|USB| vLap
  elgato-->|HDMI| switch2>Switch 2]
  dashbordPi(Dashboard Pi) -->|HDMI| switch3
  coverter===|USB 3| vLap
  vLap -->|HDMI| switch3>Switch3]
  switch3 -->|HDMI| monitor1(Monitor)
  cromecast((Chrome Cast)) -->|HDMI| switch0>Switch 0]
  webCam(WebCam) ===|USB| USBHub
  hdmiaudiosplit1 -.-|Klinke| speaker(Lautsprecher)
  elgato ===|USB 3| vLap
  funkmikro1(Funkmikro 1)
  funkmikro2(Funkmikro 2)

  classDef Elgato fill:#efefef,stroke:#000,stroke-width:1px;
  classDef Switch fill:#ffaa11,stroke:#000,stroke-width:1px;
  classDef SoundCard fill:#eeff00,stroke:#000,stroke-width:1px;
  classDef HDMIAudiosplitter fill:#eeff00:stroke:#000,stroke-width:1px;
  classDef Beamer fill:#ee00aa,stroke:#000,stroke-width:1px;
  classDef Mic fill:#ADD8E6,stroke:#000,stroke-width:1px;
  classDef Converter fill:#efefef,stroke:#000,stroke-width:1px;
  classDef Pi fill:#8A2BE2,stroke:#000,stroke-width:1px;
  classDef Free fill:#FFFFFF,stroke:#FFFFFF,stroke-width:1px;
  classDef CromeCast fill:#ffaaff,stroke:#FFFFFF,stroke-width:1px;
  classDef FunkMikro fill:#00ff00,stroke:#FFFFFF,stroke-width:1px;

  classDef NotPresent stroke:#ff0000,stroke-width:3px;

  class A cssClass;
  class elgato Elgato;
  class switch0,switch1,switch2,switch3 Switch;
  class soundcard SoundCard;
  class hdmiaudiosplit1 HDMIAudiosplitter;
  class beamer Beamer;
  class mic Mic;
  class coverter Converter;
  class dashbordPi Pi;
  class free1 Free;
  class free2 Free;
  class free3 Free;
  class cromecast CromeCast;
  class funkmikro1 FunkMikro;
  class funkmikro2 FunkMikro;
  class funkempf1 FunkMikro;
  class funkempf2 FunkMikro;
  class hdmiaudiosplit1 NotPresent;
  class hdmiaudiosplit1 NotPresent;
  class speaker NotPresent;

  linkStyle 14 stroke:#0000ff,stroke-width:2px;
  linkStyle 20 stroke:#0000ff,stroke-width:2px;
```
### Was ist auch noch gut zu haben
- Mitgliedsformulare für Beitritt
- System zur Verwaltung von Mitgliedschaften und der Mitgliedsbeiträge
- Bankkonto. Das bekommt ihr entweder bei eurer Lokalen Sparkasse oder Online bei der [GLS Bank](https://www.gls.de/gemeinnuetzige-kunden/)
- Website um Satzung, Protokolle, Formulare zu veröffentlichen (und natürlich zur Öffentlichkeitsarbeit)
- Email Adresse: Für etwaigen Kontakt zu Mitgliedern oder dem Notar

### Was muss in eine Satzung
- Vereinsname
- Ort des Vereinssitzes z.B. Flensburg
- Vereinszweck (auch wichtig für die Gemeinnützigkeit)
- Mitgliedschaft im Verein
- Beitragsordnung oder ein Verweis auf eine externe Beitragsordnung
- Regelungen für den Vorstand
- Regelungen für die Mitgliederversammlung
- Regelungen zum Eintrag und Auflösung des Vereins

### Wie schreibe ich eine gute Vereinssatzung?
Am besten siehst du dir Satzungen von Vereinen an die etwas machen wie dein geplanter Verein an. Dabei sollte auch darauf geachtet werden ob die Satzungen zu Vereinen gehören die gemeinnützig sind.

### Beitragsordnung (in der Satzung)
Die Satzung muss nach jeder Änderung neu eingetragen werden und das ist jedes mal Geld & Arbeit verbunden. Deswegen haben wir unsere Beitragsordnung von unserer Satzung separiert. Die Beitragsordnung legt fest, wie hoch der Mitgliedsbeitrag für den Verein ist und welche verschiedenen Beiträge es gibt. Rechnet am besten vorher durch wie hoch eure Kosten sind und legt danach den Mitgliedsbeitrag fest. Am besten gibt es auch einen Mitgliedsbeitrag welcher reduziert ist.

### Vereinsname
Beim Vereinsnamen seit ihr total frei, dürft euch aber natürlich nicht wie ein anderer Verein, etc... benennen. Wir haben uns für den Namen Chaostreff Flensburg entschieden weil es dieses Namensmuster schon im CCC-Umfeld gibt und einfach so verwendet werden kann.

### Adresse oder Anschrift vom Verein
Dieser kann auch eine Privat Adresse sein. Wichtig ist nur das dort Post zugestellt werden kann und diese Briefe weiter an den Verein geleitet werden. Die Adresse ist vor allem wichtig für Dokumente vom Notar, Amtsgericht und gegebenenfalls Finanzamt.

### Notar Finden
Da Notare feste Sätze für ihre Arbeit bekommen unterscheiden sich die Notare nicht wirklich im Preis. Wir haben unseren aufgrund der Entfernung ausgewählt. Ihr könnt auch den Notar bei jeder Eintragung wechseln, das führt höchsten zu ein wenig mehr Arbeit weil dort die Daten vom Vorstand und Verein noch nicht hinterlegt sind.



## Fun Facts:
### Die Abkürzung e.V.
Die Abkürzung e.V. ist für einen eingetragenen Verein nicht als offizielle Abkürzung festgeschrieben. Deswegen gibt es auf Amrum (dort wird auch Friesich gesprochen) den Öömrang Ferian i. f., für iindraanj ferian. Kopiert und Quelle: [Wikipeida](https://de.wikipedia.org/wiki/Verein#Eingetragener_Verein)


Quellen und weitere Materialien: http://www.vereinsknowhow.de/kurzinfos/leitfaden.htm
Kontakt: kontakt @ samuelbtrinkmann.de
