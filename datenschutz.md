# Datenschutzerklärung für CakeBell

**Stand: 19. Oktober 2026**

## Überblick

CakeBell („die App“) ist eine App zur Erinnerung an Geburtstage deiner Kontakte. Diese Datenschutzerklärung erklärt, welche Daten die App verarbeitet, wozu und welche Rechte du hast. Sie gilt außerdem für diese Webseite.

## Verantwortlicher

Dr. Markus Gäth  
Derkskamp 95  
48163 Münster  
E-Mail: anaiccial@icloud.com

## So löschst du deine Daten

Du kannst deine Daten auf unserem Server direkt in der App löschen. Ein Konto oder eine Anfrage beim Support brauchst du dafür nicht:

1. Öffne **CakeBell** auf deinem Smartphone
2. Gehe zum Tab **Einstellungen**
3. Scrolle nach unten und tippe auf **„Meine Daten löschen“**
4. Bestätige mit **„Löschen“**

Damit werden die synchronisierten Vornamen und Geburtstage deiner Kontakte, deine Erinnerungs-Einstellungen und der Push-Token deines Geräts sofort und endgültig aus unserer Datenbank gelöscht. Was das genau umfasst, steht unten unter [Welche Daten übertragen werden](#welche-daten-übertragen-werden). Die Erinnerungen sind danach ausgeschaltet. Wenn du sie wieder einschaltest, wird ein neuer Eintrag angelegt. **Es gibt keine zusätzliche Aufbewahrungsfrist:** Der Datensatz wird sofort entfernt und nicht nur deaktiviert.

Falls du die App schon gelöscht hast und deine Daten trotzdem löschen lassen möchtest, schreib eine E-Mail an **anaiccial@icloud.com**. Gib dabei ungefähr an, wann du die App zuletzt benutzt hast und welches Gerät du hattest (iOS/Android).

## Welche Daten die App verarbeitet

### Daten auf deinem Gerät
- **Kontaktdaten:** Die App liest Namen und Geburtstage aus dem Adressbuch deines Geräts. Vollständige Namen werden nur innerhalb der App angezeigt.
- **Kontaktfotos:** Profilbilder deiner Kontakte, sofern vorhanden. Sie werden nie übertragen.
- **Einstellungen:** Erinnerungszeit, Erinnerungsintervall, Beziehungsarten und Nachrichtenvorlieben.

Diese Daten werden lokal auf deinem Gerät gespeichert (AsyncStorage).

### Welche Daten übertragen werden
Damit Geburtstagserinnerungen zuverlässig per Push-Mitteilung ankommen, werden folgende Daten verschlüsselt an unseren Server übertragen:
- **Vorname und Geburtstag** (nur Tag und Monat) von Kontakten mit Geburtstag. Nachnamen werden nicht übertragen.
- **Die interne Kennung des Kontakts aus deinem Adressbuch**, damit ein Geburtstag, zu dem du schon gratuliert hast, als erledigt markiert werden kann.
- **Deine Erinnerungs-Einstellungen** (Uhrzeit, Intervall, ein/aus, App-Sprache und Zeitzonen-Abweichung).
- **Der Push-Token deines Geräts**, den Apple bzw. Google vergeben.

Wenn du die Erinnerungen ausschaltest, wird dein Eintrag auf dem Server sofort gelöscht. Solange sie ausgeschaltet sind, werden keine Daten übertragen.

### Was nicht übertragen wird
- Keine Nachnamen, Telefonnummern, E-Mail-Adressen oder Fotos
- Keine Daten von Kontakten ohne Geburtstag
- Keine Nachrichteninhalte oder Kommunikationsverläufe
- Keine Gerätekennungen, Standortdaten oder Nutzungsstatistiken

## Zwecke und Rechtsgrundlagen

- **Anzeige der Geburtstage und Versand der Erinnerungen:** Das ist die Funktion der App, die du nutzt. Rechtsgrundlage ist Art. 6 Abs. 1 lit. b DSGVO (Erfüllung des Vertrags über die Nutzung der App).
- **Vornamen und Geburtstage deiner Kontakte:** Hier verarbeiten wir Daten von Personen, die die App nicht selbst nutzen. Rechtsgrundlage ist Art. 6 Abs. 1 lit. f DSGVO. Das berechtigte Interesse besteht darin, dich an Geburtstage zu erinnern. Wir beschränken die Daten dabei auf Vorname und Tag/Monat des Geburtstags.
- **Persönliche Geburtstagsnachrichten:** Sie werden nur lokal auf deinem Gerät erstellt.

## Empfänger und Dienstleister

**Wir verkaufen deine Daten nicht und geben sie nicht für Werbe- oder Marketingzwecke weiter.** Für den Betrieb setzen wir folgende Dienstleister als Auftragsverarbeiter ein:

- **Amazon Web Services (AWS):** Speicherung der übertragenen Daten in einer verschlüsselten DynamoDB-Datenbank und Betrieb des Backends (AWS Lambda) in der Region Frankfurt (EU).
- **Expo (650 Industries, Inc., USA):** Zustellung der Push-Mitteilungen. Expo leitet sie an den Apple Push Notification Service (APNs) bzw. Google Firebase Cloud Messaging (FCM) weiter.

Der Text der Push-Mitteilung enthält den Vornamen des Kontakts, der Geburtstag hat (z. B. „🎂 Anna hat heute Geburtstag!“). Dieser Vorname läuft deshalb bei der Zustellung über Expo, Apple und/oder Google. Andere Kontaktdaten sind nicht in der Mitteilung enthalten. Dabei werden Daten in die USA übermittelt. Die Übermittlung an Expo erfolgt auf Grundlage der Standardvertragsklauseln der EU-Kommission (Art. 46 Abs. 2 lit. c DSGVO). Apple und Google sind nach dem EU-US Data Privacy Framework zertifiziert.

Mit Messenger-Apps (SMS, WhatsApp, Threema, Telegram) arbeitet die App nur zusammen, wenn du ausdrücklich eine Geburtstagsnachricht verschickst. Das übernimmt dann die jeweilige App auf deinem Gerät.

## Berechtigungen

Die App benötigt folgende Berechtigungen:
- **Kontakte:** um Geburtstage aus deinem Adressbuch zu lesen
- **Mitteilungen:** um Geburtstagserinnerungen per Push-Mitteilung zu senden
- **SMS** (optional): um Nachrichten über die Nachrichten-App deines Geräts zu verschicken

## Speicherdauer

- Kontaktdaten werden bei jedem Öffnen der App neu eingelesen.
- Die Geburtstagsdaten auf dem Server werden bei jeder Synchronisierung überschrieben und spiegeln nur deine aktuellen Kontakte wider.
- Die Angabe, zu welchen Geburtstagen du schon gratuliert hast, wird täglich automatisch zurückgesetzt.
- Deine Einstellungen bleiben gespeichert, bis du die App löschst oder über **Einstellungen → Meine Daten löschen** die Löschung veranlasst.
- Die Löschung in der App entfernt deinen Eintrag auf dem Server (Namen, Geburtstage, Einstellungen, Push-Token) sofort und endgültig.
- Wenn du die App deinstallierst, werden alle lokalen Daten entfernt. Dein Eintrag auf dem Server wird automatisch gelöscht, sobald sich bei einer Push-Mitteilung zeigt, dass dein Gerät nicht mehr registriert ist, spätestens aber 12 Monate nach der letzten Synchronisierung durch die App. Du kannst die Löschung außerdem jederzeit per E-Mail verlangen.

## Datensicherheit

- Lokale Daten sind durch die Sicherheitsfunktionen deines Geräts geschützt (Code, biometrische Entsperrung usw.).
- Die Daten auf dem Server liegen verschlüsselt in AWS DynamoDB in der EU (Frankfurt).
- Die gesamte Kommunikation zwischen App und Server ist per HTTPS/TLS verschlüsselt.
- Das Backend läuft auf AWS Lambda ohne dauerhaft laufende Server.

## Diese Webseite

Diese Webseite wird bei GitHub Pages gehostet (GitHub, Inc., 88 Colin P. Kelly Jr. Street, San Francisco, CA 94107, USA). Beim Aufruf der Seite verarbeitet GitHub technisch notwendige Daten, insbesondere deine IP-Adresse, um die Seite auszuliefern und die Sicherheit des Dienstes zu gewährleisten. Rechtsgrundlage ist Art. 6 Abs. 1 lit. f DSGVO. Unser berechtigtes Interesse ist die zuverlässige Bereitstellung dieser Seite. GitHub ist nach dem EU-US Data Privacy Framework zertifiziert. Weitere Informationen findest du in der [Datenschutzerklärung von GitHub](https://docs.github.com/de/site-policy/privacy-policies/github-general-privacy-statement).

Diese Webseite verwendet keine Cookies, kein Tracking und keine Analyse-Tools.

## Kontakt per E-Mail

Wenn du uns per E-Mail kontaktierst, verarbeiten wir deine Angaben, um deine Anfrage zu beantworten (Art. 6 Abs. 1 lit. b bzw. f DSGVO). Wir löschen sie, sobald die Anfrage erledigt ist und keine gesetzlichen Aufbewahrungspflichten bestehen.

## Deine Rechte

Du hast nach der DSGVO das Recht auf:
- **Auskunft** über die zu dir gespeicherten Daten (Art. 15)
- **Berichtigung** unrichtiger Daten (Art. 16)
- **Löschung** (Art. 17). In der App geht das jederzeit über **Einstellungen → Meine Daten löschen**.
- **Einschränkung der Verarbeitung** (Art. 18)
- **Datenübertragbarkeit** (Art. 20)
- **Widerspruch** gegen Verarbeitungen, die auf Art. 6 Abs. 1 lit. f DSGVO beruhen (Art. 21)
- **Beschwerde** bei einer Datenschutz-Aufsichtsbehörde (Art. 77), insbesondere in dem Mitgliedstaat, in dem du wohnst oder arbeitest.

Außerdem kannst du:
- Berechtigungen jederzeit in den Einstellungen deines Geräts widerrufen
- **Einstellungen → Erinnerungen aktivieren** ausschalten. Dann wird dein Eintrag auf dem Server sofort gelöscht, und es werden keine Namen und Geburtstage mehr übertragen.
- Alle Daten auf deinem Gerät löschen, indem du die App deinstallierst

Für alle Anfragen genügt eine E-Mail an **anaiccial@icloud.com**.

## Kinder

Die App richtet sich an ein allgemeines Publikum. Wir erheben nicht wissentlich Daten von Kindern unter 13 Jahren.

## Änderungen

Wir passen diese Datenschutzerklärung an, wenn sich die App oder die Rechtslage ändert. Das Datum oben zeigt den aktuellen Stand.
