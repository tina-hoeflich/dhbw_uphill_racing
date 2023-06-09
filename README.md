# DHBW_Uphill_Racing

DHBW_Uphill_Racing ist ein Projekt, das im Rahmen der Studienarbeit an der Dualen Hochschule Baden-Württemberg in Stuttgart entwickelt wurde. Es handelt sich um ein Rennspiel, das mit einem Smart Trainer über die Software Sensor Wrangler verbunden werden kann. Darüber hinaus kann das Spiel Signale an ein Pavlok Armband senden, wenn die Hersteller-API verfügbar ist. Wenn keine Verbindung zu einem Smart Trainer besteht, kann das Spiel auch mit den Pfeiltasten auf der Tastatur gespielt werden.

## Voraussetzungen
- [Unity](https://unity.com/de)
- [Sensor Wrangler](https://github.com/Doomsdan/SensorWrangler)
- Ein Pavlok Armband (optional)

## Installation und Ausführung

1. Laden Sie das Repository herunter und entpacken Sie es in einem Verzeichnis Ihrer Wahl.
2. Installieren Sie SensorWrangler von [https://github.com/Doomsdan/SensorWrangler](https://github.com/Doomsdan/SensorWrangler)
3. Fügen Sie eine Datei mit dem Namen `.bazeliskrc` hinzu und fügen Sie `USE_BAZEL_VERSION=4.2.2` ein.
4. Bauen Sie das Projekt mit Bazelisk: führen Sie im Hauptverzeichnis des Projekts den Befehl `bazelisk build //:Gui` aus.
5. Navigieren Sie in das `bazel-bin` Verzeichnis mit `cd bazel-bin`.
6. Führen Sie das Programm mit `./Gui.exe` (Windows) oder `./Gui` (Linux/Mac) aus.
7. Fügen Sie einen Leistungssensor hinzu.
8. Starten Sie den Socket an Port 8000.

## Nutzung

Stellen Sie eine Verbindung zu Ihrem Smart Trainer über Sensor Wrangler her und beginnen Sie das Spiel. Das Spiel sendet Signale an Ihr Pavlok Armband basierend auf den Daten, die es vom Smart Trainer und Sensor Wrangler erhält.

Wenn keine Verbindung zu einem Smart Trainer besteht, kann das Spiel mit den Pfeiltasten auf der Tastatur gespielt werden.

Viel Spaß beim Spielen!
