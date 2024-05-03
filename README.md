# LA1304


Greub, Lucena Losada, Manser

## 1 Informieren


### 1.1 Ihr Projekt

Ein vielseitiger Zahlensystem-Rechner zur Umwandlung zwischen Hexadezimal, Dezimal und Binär.

Der Rechner sollte zwischen Hexadezimal, dezimal und Binär umrechnen können, es sollte ein GUI haben sowie in c# geschrieben werden.

### 1.2 User Stories

| US-№ | Verbindlichkeit | Typ  | Beschreibung                       |
| ---- | --------------- | ---- | ---------------------------------- |
|1|	Muss|	Funktional|	Als Nutzer möchte ich Dezimalzahlen in Binär umwandeln, um Berechnungen im Binärsystem durchzuführen.|
|2|	Muss|	Funktional|	Als Nutzer möchte ich Binärzahlen in Dezimal umwandeln, um alltägliche Zahlen zu verstehen.|
|3|	Muss|	Funktional|	Als Nutzer möchte ich Hexadezimalzahlen in Dezimal umwandeln, um einfacher mit Hardware-naher Software zu arbeiten.|
|4|	Muss|	Funktional|	Als Nutzer möchte ich Dezimalzahlen in Hexadezimal umwandeln, um Farbcodes für Webseiten zu generieren.|
|5|	Muss|	Funktional|	Als Nutzer möchte ich Binärzahlen in Hexadezimal umwandeln, um Fehlermeldungen zu decodieren.|
|6| muss| Funktional | Als Nutzer möchte ich Hexadezimalzahlen in Binär umwandeln.|
|7|	Kann|	Qualität|	Als Entwickler möchte ich, dass der Code gut kommentiert ist, damit zukünftige Wartungen leichter fallen.|
|8|	Muss|	Qualität|	Als Nutzer möchte ich eine klare und intuitive Benutzeroberfläche haben, damit ich leicht navigieren kann.|
|9|	Kann|	Rand|	Als Nutzer möchte ich eine Historie meiner letzten Umwandlungen sehen, um schnell auf frühere Ergebnisse zurückgreifen zu können.|
|10|	Muss	|Funktional|	Als Nutzer möchte ich Fehlermeldungen erhalten, wenn ich ungültige Eingaben mache, um meine Eingaben korrigieren zu können.|


### 1.3 Testfälle

| TC-№ | Ausgangslage | Eingabe | Erwartete Ausgabe |
| ---- | ------------ | ------- | ----------------- |
|1.1|	Start des Programms|	10 (Dezimal)|	1010 (Binär)|
|2.1|	Start des Programms|	1010 (Binär)|	10 (Dezimal)|
|3.1|	Start des Programms|	1A (Hex)	26| (Dezimal)|
|4.1|	Start des Programms|	255 (Dezimal)|	FF (Hex)|
|5.1|	Start des Programms|	1010 (Binär)|	A (Hex)|
|6.1|	Start des Programms|	A (Hex)|	1010(Binär)|
| 8.1| Start des Programms| - | Klare UI Sichtbar |
|9.1|	Mehrfache Eingaben|	10 Umwandlungen|	Anzeige der Historie|
|10.1|	Falsche Eingabe|	2X (Hex)|	Fehlermeldung|


## 2 Planen

| AP-№ | Frist | Zuständig | Beschreibung | geplante Zeit |
| ---- | ----- | --------- | ------------ | ------------- |
| 1.A  | 19.04.2024| Manser Alberto | Dezimal -> Binär       | 45|
| 2.A  | 19.04.2024| Manser Alberto | Binär -> Dezimal       | 45|
| 3.A  | 19.04.2024| Lucena Samuel  | Hexadezimal -> Dezimal | 2 x 45 |
| 4.A  | 19.04.2024| Lucena Samuel  | Dezimal -> Hexadezimal | 2 x 45 |
| 5.A  | 19.04.2024| Manser Alberto | Hexadezimal -> Binär   | 2 x 45|
| 6.A  | 19.04.2024| Manser Alberto | Binär -> Hexadezimal   | 2 x 45|
| 7.A  | 26.04.2024| Greub Manuel | Code mit Kommentaren Bestücken | 2 x 45 |
| 8.A  | 26.04.2024| Greub Manuel | GUI implementieren und Rechner einfügen | 2 x 45 |
| 10.A | 26.04.2024| Greub Manuel | Implementierung Fehlerabfang | 45 |

Total: 15 x 45


## 3 Entscheiden

Wegen komplikationen haben wir uns entschieden die Userstory 9 sowie den Testfall 9.1 nicht zu implementieren

## 4 Realisieren

| AP-№ | Datum | Zuständig | geplante Zeit | tatsächliche Zeit |
| ---- | ----- | --------- | ------------- | ----------------- |
| 1.A  | 5.04.2024 | Manser Alberto |  45 |  30 |
| 2.A  | 5.04.2024 | Manser Alberto |  45 |  30 |
| 3.A  | 5.04.2024 | Lucena Samuel  | 2 x 45 | 2 x 45 |
| 4.A  | 5.04.2024 | Lucena Samuel  | 2 x 45 | 2 x 45 |
| 5.A  |5.04.2024 | Manser Alberto | 2 x 45 | 60 |
| 6.A  | 5.04.2024 | Manser Alberto | 2 x 45 | 45 |
| 7.A  | 26.04.2024 | Greub Manuel | 45 | 20 |
| 8.A | 19.04.2024 | Greub Manuel | 2 x 45 | 3 x 45 |
| 10.A| 19.04.2024 | Greub Manuel | 45 | 30 |

## 5 Kontrollieren

| TC-№ | Datum | Resultat | Tester |
| ---- | ----- | -------- | ------ |
| 1.1  | 26.04.2024 | Funktioniert|Lucena Samuel|
| 2.1  | 26.04.2024 | Funktioniert|Lucena Samuel |
| 3.1|26.04.2024|Funktioniert|Lucena Samuel|
| 4.1 |26.04.2024|Funktioniert|Lucena Samuel|
| 5.1 |26.04.2024|Funktioniert|Lucena Samuel|
|6.1 |26.04.2024|Funktioniert|Lucena Samuel|
|8.1|26.04.2024|Funktioniert|Lucena Samuel|
|10.1|26.04.2024|Funktioniert Nicht|Lucena Samuel|

Das meiste im Programm funktioniert, alle Berechnungen funktionieren, der Failsafe jedoch nicht.

