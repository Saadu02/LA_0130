# Projekt-Dokumentation

LA_0130 von Nicola Karrer und Sathana Suganthasri

| Datum | Version | Zusammenfassung                                              |
| ----- | ------- | ------------------------------------------------------------ |
| 10.01.25 | 0.0.1   | Projektantrag und Dokumentation erstellt |
| 17.01.25 | 0.0.2   | Programm erstellt und Raster so wie Punkte implementiert |
| 24.01.25 | 0.0.3   | X |

## 1 Informieren

### 1.1 Ihr Projekt

Ein Spiel, in dem man ein vorbestimmtes Grid hat und darin Punkte verbinden muss. Es hat immer nur zwei Punkte pro Farbe und auf einem Feld darf immer nur eine Farbe sein.

Normalerweise spielen wir oft das Spiel "Flow Free". Wir haben uns gedacht, dass wir es selbst entwickeln könnten, da es für uns neu etwas neues ist, in dieser Art zu programmieren. Unser Ziel ist es zunächst, das Spiel funktionsfähig zu machen, so dass man als Spieler Punkte verbinden kann. Je nach zeitlicher Verfügbarkeit werden wir weitere Funktionen entwickeln, um das Spiel interessanter und unterhaltsamer zu gestalten. Mit diesem Projekt möchten wir unsere Kenntnisse in der Programmiersprache C# anwenden und uns intensiver mit WinForms auseinandersetzen.

### 1.2 User Stories

| US-№ | Verbindlichkeit | Beschreibung                       |
| ---- | --------------- | ---------------------------------- |
| 1  | Funktionalität | Als Benutzer möchte ich, dass das Programm automatisch ein Spiel erstellt |
| 2  | Funktionalität | Als Benutzer möchte ich, dass die Spiele immer wieder neu sind, damit das spielen nicht langweilig wird |
| 3  | Funktionalität | Als Benutzer möchte ich Linien verbinden können, um das Spiel zu lösen |
| 4  | Funktionalität | Als Benutzer möchte ich, dass die Linien unterschiedliche Farbe haben, damit ich weiss, welche Punkte ich verbinden muss |
| 5  | Funktionalität | Als Benutzer möchte ich, dass es einen Knopf gibt, um das Spiel neustarten zu können |
| 6  | Qualität | Als Benutzer möchte ich, dass es genau eine Möglichkeit gibt das Spiel zu lösen |
| 7  | Qualität | Als Benutzer möchte ich, dass ich die Bildschirmgrösse anpassen kann, damit ich es in einem kleineren oder grösseren Fenster spielen kann |
| 8  | Qualität | Als Benutzer möchte ich, dass das Design benutzerfreundlich ist. |


### 1.3 Testfälle

| TC-№ | Ausgangslage | Eingabe | Erwartete Ausgabe |
| ---- | ------------ | ------- | ----------------- |
| 1.1  | Programm offen | Programm starten | Menu öffnet sich|
| 1.2  | Menu geöffnet | Spiel starten | Raster wird generiert |
| 2.1  | Spiel geschafft | Neues Spiel | Weiteres neues Spiel wird generiert |
| 3.1  | Spiel gestartet | Verbinde zwei Punkte | Linie wird gezogen |
| 4.1  | Menu geöffnet | Spiel starten | Punkte werden in verschiedenen Farben angezeigt |
| 5.1  | Spiel gestartet | Spiel geschafft | Neustart Knopf wird angezeigt |
| 6.1  | Menu geöffnet | Spiel starten | 1 Möglichkeit das Spiel zu lösen |
| 7.1  | Spiel gestartet | Fenster anpassen | Raster wird mit angepasst |
| 8.1  | Proframm offen | Programm starten | Funktionsweise klar ohne fremde Hilfe |

### 1.4 Diagramme

<img src="https://github.com/user-attachments/assets/6f87a13f-9aaa-407a-abb6-b49fe6eabc81" alt="Bild" width="600" />

10.01

![image](https://github.com/user-attachments/assets/d13243e6-cbaa-4459-b30a-2d78b9e5ed25)

17.01



## 2 Planen

| AP-№ | Frist | Zuständig | Beschreibung | geplante Zeit |
| ---- | ----- | --------- | ------------ | ------------- |
| 0.A  | 10.01.2025 | Alle | Projektantrag, Planung, erste Skizze | 180min |
| 1.A  | 17.01.2025 | Alle | Automatisch ein Spiel erstellen | 30min |
| 1.B  | 17.01.2025 | Alle | Raster erstellen | 60min |
| 3.A  | 17.01.2025 | Alle | Linien verbinden | 90min |
| 2.A  | 24.01.2025 | Sathana | Neue verbindungsmöglichkeiten | 180min |
| 4.A  | 24.01.2025 | Nicola | Unterschiedliche Farben für Linien | 180min |
| 5.A  | 14.02.2025 | Sathana | Neustart-Knopf | 180min |
| 6.A  | 14.02.2025 | Nicola | Nur eine Möglichkeit | 180min |
| 7.A  | 21.02.2025 | Sathana | Bildschirmgrösse anpassung | 90min |
| 8.A  | 21.02.2025 | Nicola  | Design | 90min |
| X.X  | 21.02.2025 | Sathana | XX | 90min|
| X.X  | 21.02.2025 | Nicola | XX | 90min|
| X.X  | 28.02.2025 | Beide | XX | 180min|
| X.X  | 07.03.2025 | Beide | XX | 180min|


## 3 Entscheiden

10.01. Wir haben uns dazu entschieden, das Programm auf VS in C# zu machen und dabei Winforms zu benutzen.

## 4 Realisieren

| AP-№ | Datum | Zuständig | geplante Zeit | tatsächliche Zeit |
| ---- | ----- | --------- | ------------- | ----------------- |
| 0.A  | 10.01.25 | Alle | 180min | 180min |
| 1.A  | 17.01.25 | Alle | 30min | 10min |
| 1.B  | 17.01.25 | Alle | 60min | 80min |
| 3.A  | 17.01.25 | Alle | 90min | 90min |
| 2.A  | |  |  |  |
| 4.A  | |  |  |  |
| 5.A  | |  |  |  |
| 6.A  | |  |  |  |
| 7.A  | |  |  |  |
| 8.A  | |  |  |  |

## 5 Kontrollieren

### 5.1 Testprotokoll

| TC-№ | Datum | Resultat | Tester |
| ---- | ----- | -------- | ------ |
| 1.1  | 07.03.2025 |  | Sathana Suganthasri |
| 1.2  | 07.03.2025 |  | Sathana Suganthasri |
| 3.1  | 07.03.2025 |  | Nicola Karrer |
| 2.1  | 07.03.2025 |  | Sathana Suganthasri |
| 4.1  | 07.03.2025 |  | Nicola Karrer|
| 5.1  | 07.03.2025 |  | Sathana Suganthasri |
| 6.1  | 07.03.2025 |  | Nicola Karrer |
| 7.1  | 07.03.2025 |  | Sathana Suganthasri |
| 8.1  | 07.03.2025 |  | Nicola Karrer |
