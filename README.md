# DHBW Uphill Racing

DHBW_Uphill_Racing ist ein Projekt, das im Rahmen der Studienarbeit an der Dualen Hochschule Baden-Württemberg in Stuttgart entwickelt wurde. Es handelt sich um ein Rennspiel, das mit einem Smart Trainer über die Software Sensor Wrangler verbunden werden kann. Darüber hinaus kann das Spiel Signale an ein Pavlok Armband senden, wenn die Hersteller-API verfügbar ist. Wenn keine Verbindung zu einem Smart Trainer besteht, kann das Spiel auch mit den Pfeiltasten auf der Tastatur gespielt werden.


## Voraussetzungen
- [Unity](https://unity.com/de)
- [Sensor Wrangler](https://github.com/Doomsdan/SensorWrangler)
- Keine Störenden ANT+ Signale in der Nähe
- Ein Pavlok Armband (optional)

## Installation und Ausführung

1. Laden Sie das Repository herunter und entpacken Sie es in einem Verzeichnis Ihrer Wahl.
2. Installieren Sie SensorWrangler von [https://github.com/Doomsdan/SensorWrangler](https://github.com/Doomsdan/SensorWrangler)

3. Fügen Sie eine Datei mit dem Namen `.bazeliskrc` hinzu und fügen Sie `USE_BAZEL_VERSION=4.2.2` ein.
4. Bauen Sie das Projekt mit Bazelisk: führen Sie im Hauptverzeichnis des Projekts den Befehl `bazelisk build //:Gui` aus.
5. Navigieren Sie in das `bazel-bin` Verzeichnis mit `cd bazel-bin`.
6. Führen Sie das Programm mit `./Gui.exe` (Windows) aus.
7. Fügen Sie einen Leistungssensor hinzu.
8. Starten Sie den Socket an Port 8000 über die GUI der SensorWrangler Software.

## Nutzung

Stellen Sie erst eine Verbindung zu Ihrem Smart Trainer über Sensor Wrangler her und beginnen Sie das Spiel durch ausführen der Datei `Studienarbeit Uphill Racing.exe`. Das Spiel nutzt dann die Daten, die es über die Socketverbindung bekommt, um das Fahrrad zu bewegen und sendet Signale an Ihr Pavlok Armband basierend auf den Daten, die es vom Smart Trainer und Sensor Wrangler erhält.

Die Regel lautet: Schneller ist nicht immer besser! Das Ziel ist es, ein möglichst effektives Ausdauertraining zu absolvieren - nicht zu langsam, nicht zu schnell. Dies wird sich im erreichten Score wiederspielgeln!
Wenn das Spiel beendet ist, muss ein neuer SocketRecorder auf der Seite von SensorWrangler neu gestartet werden.

Wenn keine Verbindung zu einem Smart Trainer besteht, kann das Spiel mit den Pfeiltasten auf der Tastatur gespielt werden. Dies wird dann als Hinweis auf dem Bildschirm angezeigt.

Am Ende des Spiels können Sie Ihren Namen angeben, um in die Rangliste aufgenommen zu werden. 
Viel Spaß beim Spielen!

![ablaufdiagramm_allgemein](https://github.com/tina-hoeflich/dhbw_uphill_racing/assets/44570841/717c233b-7994-45bb-9fc9-5fcac8d86863)

