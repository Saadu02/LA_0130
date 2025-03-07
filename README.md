# Projekt-Dokumentation

LA_0130 von Nicola Karrer und Sathana Suganthasri

| Datum | Version | Zusammenfassung                                              |
| ----- | ------- | ------------------------------------------------------------ |
| 10.01.25 | 0.0.1   | Projektantrag und Dokumentation erstellt |
| 17.01.25 | 0.0.2   | Programm erstellt und Raster so wie Punkte implementiert |
| 24.01.25 | 0.1.0   | Punkte mit Linie verbinden |
| 14.02.25 | 0.1.1   | Keine diagonalen Linien-Verbindungen und unmögliche Generierungen verhindert |
| 21.02.25 | 0.1.2   | Linien-Verbindungen mit korrekter Farbe über andere Felder und nur noch Generierungen mit einer Lösungsmöglichkeit |

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


### 1.3 Testfälle

| TC-№ | Ausgangslage | Eingabe | Erwartete Ausgabe |
| ---- | ------------ | ------- | ----------------- |
| 1.1  | Programm offen | Programm starten | Menu öffnet sich|
| 1.2  | Menu geöffnet | Spiel starten | Raster wird generiert |
| 2.1  | Spiel geschafft | Neues Spiel | Weiteres neues Spiel wird generiert |
| 3.1  | Spiel gestartet | Verbinde zwei Punkte | Linie wird gezogen |
| 3.2  | Spiel gestartet | Verbinde zwei Punkte | Keine falschen Verbindungsmöglichkeiten |
| 4.1  | Menu geöffnet | Spiel starten | Punkte werden in verschiedenen Farben angezeigt |
| 5.1  | Spiel gestartet | Spiel geschafft | Neustart Knopf wird angezeigt |
| 6.1  | Menu geöffnet | Spiel starten | 1 Möglichkeit das Spiel zu lösen |

### 1.4 Diagramme

<img src="https://github.com/user-attachments/assets/6f87a13f-9aaa-407a-abb6-b49fe6eabc81" alt="Skizze Produkt" width="500" />

10.01

<img src="https://github.com/user-attachments/assets/d13243e6-cbaa-4459-b30a-2d78b9e5ed25" alt="Skizze Meilenstein" width = "1000" />

17.01



## 2 Planen

| AP-№ | Frist | Zuständig | Beschreibung | geplante Zeit |
| ---- | ----- | --------- | ------------ | ------------- |
| 0.A  | 10.01.2025 | Alle | Projektantrag, Planung, erste Skizze | 180min |
| 1.A  | 17.01.2025 | Alle | Automatisch ein Spiel erstellen | 30min |
| 1.B  | 17.01.2025 | Alle | Raster erstellen | 60min |
| 3.A  | 17.01.2025 | Alle | Linien verbinden | 90min |
| 3.A  | 24.01.2025 | Sathana | Linienverbindungslogik | 180min |
| 4.A  | 24.01.2025 | Nicola | Linien werden in verschiedenen Farben angezeigt | 180min |
| 3.B  | 14.02.2025 | Sathana | Keine falschen Verbindungsmöglichkeiten | 180min |
| 6.A  | 14.02.2025 | Nicola | Keine unmöglichen Generierungen | 180min |
| 3.B  | 21.02.2025 | Sathana | Keine doppelten Verbindungsmöglichkeiten | 180min |
| 6.A  | 21.02.2025 | Nicola | Generierungen mit nur 1 Lösungsmöglichkeit | 180min |
| 3.B  | 28.02.2025 | Sathana | Restliche Verbindugnsfehler | 90min |
| 2.A  | 28.02.2025 | Nicola | Neustartknopf | 90min |
| 0.B  | 28.02.2025 | Alle | Testfälle | 90min|
| 0.C  | 07.03.2025 | Alle | Dokumentation | 180min|


## 3 Entscheiden

10.01. Wir haben uns dazu entschieden, das Programm auf VS in C# zu machen und dabei Winforms zu benutzen.

14.02.2025: Die Pakete 3.B und 6.A mussten wir eine Woche später erneut planen, da wir die gesamte Logik noch nicht ganz richtig implementieren konnten. Zum einen kann man die Linien immer noch über Punkte und andere Farben ziehen und auf der anderen Seite generiert es immer noch Spiele mit falschen/mehreren Lösungsmöglichkeiten.

## 4 Realisieren

| AP-№ | Datum | Zuständig | geplante Zeit | tatsächliche Zeit |
| ---- | ----- | --------- | ------------- | ----------------- |
| 0.A  | 10.01.25 | Alle | 180min | 180min |
| 1.A  | 17.01.25 | Alle | 30min | 10min |
| 1.B  | 17.01.25 | Alle | 60min | 80min |
| 3.A  | 17.01.25 | Alle | 90min | 90min |
| 3.A  | 24.01.25 | Alle | 90min | 45min |
| 2.A  | 24.01.25 | Sathana | 180min | 135min |
| 4.A  | 24.01.25 | Nicola | 180min | 135min |
| 5.A  | 14.02.25 | Sathana | 180min | 180min |
| 6.A  | 14.02.25 | Nicola | 180min | 180min |
| 5.A  | 21.02.25 | Sathana | 180min | 180min |
| 6.A  | 21.02.25 | Nicola | 180min | 180min |

## 5 Kontrollieren

### 5.1 Testprotokoll

| TC-№ | Datum | Resultat | Tester |
| ---- | ----- | -------- | ------ |
| 1.1  | 28.02.2025 |  | Sathana Suganthasri |
| 1.2  | 28.02.2025 |  | Sathana Suganthasri |
| 3.1  | 28.02.2025 |  | Nicola Karrer |
| 2.1  | 28.02.2025 |  | Sathana Suganthasri |
| 4.1  | 28.02.2025 |  | Nicola Karrer|
| 5.1  | 28.02.2025 |  | Sathana Suganthasri |
| 6.1  | 28.02.2025 |  | Nicola Karrer |
| 7.1  | 28.02.2025 |  | Sathana Suganthasri |
| 8.1  | 28.02.2025 |  | Nicola Karrer |
