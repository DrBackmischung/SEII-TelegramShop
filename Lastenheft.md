# Inhalt

- [1) Zielbestimmungen](#ziel)
  - [1.1) Muss-Kriterien](#muss)
  - [1.2) Soll-Kriterien](#soll)
- [2) Einsatz](#einsatz)
  - [2.1) Anwendungsbereich](#anwendung)
  - [2.2) Zielgruppen](#zielgruppen)
  - [2.3) Betriebsbedingung](#betriebsbedingung)
  
<a name="ziel"></a>
## 1) Zielbestimmungen

Im folgenden sind die Zielbestimmungen definiert, aufteilet in Muss- und Soll-Kriterien.

<a name="muss"></a>
### 1.1) Muss-Kriterien

Der Kunde muss
- das Sortiment ansehen können
- die Details von einzelnen Produkten sehen können
- die Produkte in einen Warenkorb legen können
- den Warenkorb bearbeiten können
- die Bestellung abschicken können
- Liefer- & Rechnungsadressen eingeben können
- Bezahlinformationen eingeben können
- Lieferstatus überwachen können
- die Bestellung widerufen/stornieren können
- die Möglichkeit haben, den Support kontaktieren zu können

Der Admin muss
- das Sortiment anlegen können
- die Bestellungen ansehen können
- die Funktionalitäten des Shops verändern können
- Nachrichten des Shops anpassen können
- Supportanfragen annehmen können
- Supportanfragen bearbeiten können

<a name="soll"></a>
### 1.2) Soll-Kriterien

Der Kunde soll
- die Anwendung barrierefrei nutzen können
- Liefer- & Rechnungsadressen im Konto speichern können
- Bezahlinformationen im Konto speichern können
- die Sprache der Anwendung ändern können

Der Admin soll
- Übersetzungen hinzufügen können
- Workflows ändern können

<a name="einsatz"></a>
## 2) Einsatz

Im folgenden ist der Einsatz der Applikation definiert.

<a name="anwendung"></a>
### 2.1) Anwendungsbereich

Die Anwendung soll als B2C-Service angeboten werden und eine schnelle, unkomplizierte Möglichkeit bieten, dass vor allem kleinere Unternehmen schnell ihre Ware verkaufen können. Die Anwendung soll im alltäglichen Gebrauch eingesetzt werden, um schnell zB. Waren zu kaufen oder Essen zu bestellen.

<a name="zielgruppen"></a>
### 2.2) Zielgruppen

Hier Personas aus der User Story einfügen

<a name="betriebsbedingungen"></a>
### 2.3) Betriebsbedingungen

Das System soll mit einer Internetverbindung von überall aus bedienbar und konfigurierbar sein. Dafür soll das System eine maximale Uptime haben, damit durchgehend von den Admins auf die Bots zugegriffen werden kann. Auch sollen Bezahl- und Bestellvorgänge nicht einfach abbrechen, weshalb eine maximale Uptime wichtig ist. Auch nachts sollen die Bots/Shops online sein, wobei in frühen Morgenstunden (zwischen 3-4 Uhr) Wartungsarbeiten stattfinden könnten, da dort sehr geringer User-Traffic zu erwarten ist.

<a name="umgebung"></a>
## 3) Umgebung

<a name="backend"></a>
### 3.1) Backend

Die Architektur wird eine Microservice-Architektur sein. Dies hat den Grund, dass solche Systeme skalable und zukunftssicher sind. Es gibt eine Haupt-Applikation und verschiedene Services für verschiedene Funktionalitäten (Support, Bestellung, Profil, etc.). Diese sind alle voneinander unabhängig und können dementsprechend auch mit verschiedenen Programmiersprachen oder Techniken entwickelt werden. Die Kommunikation soll über REST laufen, da dies weitgehend bekannt und als weitgehend gut akzeptiert wird. 

<a name="frontend"></a>
### 3.2) Frontend

Das Frontend basiert auf bereits bekannten und berühmten Apps für Telegram. Das Design ist simpel und intuitiv, so einfach wie möglich und so komplex wie nötig. Durch einfache Auswahlfenster und Entscheidungsdialoge mit dem Shop soll das Design so einfach wie möglich sein. Große Anpassungen sind nicht nötig bzw. müssen nicht möglich sein.

<a name="hosting"></a>
### 3.3) Hosting

Das Hosting für Telegram-Bots ist auf AWS geplant. Dort gibt es zum Hosten, zum Loggen und zum Überwachen eine Vielzahl von Apps, die effizient die Arbeitsschritte erleichtern.

<a name="architektur"></a>
### 3.4) Architektur

kommt noch von Yasin & Marsl

<a name="daten"></a>
## 4) Daten

Die Daten werden relational in Datenbanken gespeichert. Diese sind in Tabellen verfügbar und können über SQL ausgelesen werden. Es sind pro Shop im Schnitt 1.000-10.000 Datensätze zu Bestellungen, 500-5.000 Datensätze zu Profilen sowie Datensätze für 20-100 Produkte und deren verfügbarkein zu erwarten. In den ersten Jahren sind Kapazitäten für bis zu 10.000 Shops geplant. Die Daten müssen mindestens so lange gehalten werden, wie nach Gesetzt für zB. Buchhaltung vorgeschrieben ist. 

<a name="ui"></a>
## 5) Benutzeroberfläche

Die Benutzeroberfläche für die Hauptanwendung ist das Chat-Fenster von Telegram. Dort kann mit Bildern und Dialogfenstern die Applikation gesteuert werden. Diese Bilder und das Design der Dialoge, Nachrichten und Popups sollen intuitiv und einfach sein, nicht zu sehr rausstechen und schlicht sein. 

<a name="qualität"></a>
## 6) Qualität

Die Anwendung soll qualitätativ hochwertig sein. Die Anwendung soll so implementiert werden, dass sie eine minimale Ausfall- und Absturzquote hat, damit der Enduser keine Probleme mit der Anwendung bekommt. Das Design soll so intuitiv und objektiv schön wie möglich gehalten werden, damit der Enduser die Applikation nicht hässlich findet. Außerdem soll der Code eine gewisse Qualität aufweisen, dies wird durch Code Testing mit einer maximalen Coverage sichergestellt.

<a name="funktionen"></a>
## 7) Funktionen

Hier User Story einfügen

<a name="ergänzungen"></a>
## 8) Ergänzungen

Zum jetzigen Zeitpunkt keine Ergänzungen.

