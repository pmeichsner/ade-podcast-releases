# ADE Podcast

Automatischer Podcast-Kameraschnitt für Adobe Premiere Pro 27.0 unter Windows x64.

**[Aktuellen Installer herunterladen](https://github.com/pmeichsner/ade-podcast-releases/releases/latest)**

## Installation

1. Projekte speichern und Premiere Pro schließen.
2. Eine bisher im UXP Developer Tool geladene ADE-Podcast-Instanz entladen.
3. Die Datei **ADE-Podcast-1.0.0-Setup-x64.exe** aus dem Release starten.
4. Premiere öffnen und **Fenster → UXP Plugins → ADE Podcast** wählen.

Voraussetzungen: Premiere Pro 27.0, Creative Cloud Desktop und Windows x64 mit .NET Framework 4.8. Panel, lokale Engine und Adobe-Brücke sind im Installer enthalten. ADE Captions und das UXP Developer Tool werden zum Betrieb nicht benötigt.

## Kameraschnitt

Synchronisierte Kameraspuren und separate Mikrofonspuren zuordnen, die aktive Sequenz einlesen und **Podcast schneiden** starten. ADE erstellt eine Sequenzkopie und aktiviert die Kamera der sprechenden Person. Bei Überschneidungen verwendet es die Totale. Zusätzliche Totalen werden unabhängig davon nach einem zufälligen Zeitplan gesetzt.

- 1–8 Sprecher und 2–8 Kameras, Presets und passende Audiozeilen.
- Jede Kameraspur erhält nur die für ihre eigenen Aktivierungswechsel benötigten Schnitte.
- Während des Laufs wird der Schnittbutton zum roten **Abbrechen**-Button.
- Audiospuren bleiben erhalten. Die Audioanalyse läuft lokal und verwendet gefilterte Pegel; den erzeugten Rohschnitt vor dem Export prüfen.

Jede Kamera muss die ganze Sequenz ohne Lücken abdecken. Mehrere Kameras können denselben Sprecher tragen; für dessen Nahaufnahme verwendet Version 1.0.0 die erste zugeordnete Kamera.

## Automatische Updates

Die Update-Quelle dieses Repositorys ist voreingestellt. Auf Schnittrechnern ist kein GitHub-Konto erforderlich. Der Updater prüft signierte Metadaten und SHA-256-Prüfsummen, lädt geänderte Komponenten und installiert erst bei geschlossenem Premiere. Bei einem fehlgeschlagenen Update wird der vorherige Stand wiederhergestellt. Ohne Internet bleibt die installierte Version nutzbar.

Im Startmenü stehen **ADE Podcast Engine**, **ADE Podcast Updates** und **ADE Podcast Jetzt aktualisieren** bereit. Eine leere Update-Quelle deaktiviert automatische Downloads. Installationsordner: `%LOCALAPPDATA%\Programs\ADE Podcast\managed`.

ADE Podcast und ADE Captions arbeiten mit normalen Premiere-Sequenzen. Sie besitzen jeweils eigene Laufzeiten, Einstellungen und Updates und funktionieren unabhängig voneinander.

Dieses Repository verteilt Installationspakete und Updates. Der Projektquellcode wird hier nicht veröffentlicht.
