# Gambio Security Patches

**Deutsch** · [English](#gambio-security-patches-english)

Dieses Repository stellt Sicherheitspatches für Gambio-Shopversionen zum Download bereit.
Es enthält ausschließlich die Patch-Pakete und die zugehörigen Hinweise, keinen Shop-Quellcode.

> **Warum hier?** Wir haben aktuell mit einem Ausfall unseres Kundenportals, des Forums und des Blogs zu tun. Aufgrund verdächtiger Aktivitäten auf unserem Webserver haben wir die betroffene Hardware vorsorglich und kontrolliert heruntergefahren.
Wir prüfen unsere Systeme sorgfältig und nehmen die einzelnen Dienste anschließend Schritt für Schritt wieder in Betrieb. Den aktuellen Stand findest Du jederzeit unter [www.gambio.de/status](https://www.gambio.de/status).

## Verfügbare Patches

**Security Update 2026-09 v1.0** (14.09.2026) schließt eine Sicherheitslücke in der StyleEdit-Anmeldung.
Es gibt eine ZIP-Datei je Versionsbereich. Wähle die Datei, die zu deiner Shopversion passt, und klicke
auf den Dateinamen, um sie herunterzuladen.

| Deine Shopversion | Download |
|---|---|
| **26.04.2 – 26.09.1** | [gambio-security-update-2026-09-v1.0_v26.04.2-v26.09.zip](https://github.com/gambio/security-patches/releases/download/security-update-2026-09-v1.0/gambio-security-update-2026-09-v1.0_v26.04.2-v26.09.zip) |
| **26.04.1** | [gambio-security-update-2026-09-v1.0_v26.04.1.zip](https://github.com/gambio/security-patches/releases/download/security-update-2026-09-v1.0/gambio-security-update-2026-09-v1.0_v26.04.1.zip) |
| **4.9.x, 5.0.x, 5.1.0.0, 26.03.0 – 26.04.0** | [gambio-security-update-2026-09-v1.0_v4.9-v26.04.0.zip](https://github.com/gambio/security-patches/releases/download/security-update-2026-09-v1.0/gambio-security-update-2026-09-v1.0_v4.9-v26.04.0.zip) |
| **4.3.x – 4.8.x** | [gambio-security-update-2026-09-v1.0_v4.3-v4.8.zip](https://github.com/gambio/security-patches/releases/download/security-update-2026-09-v1.0/gambio-security-update-2026-09-v1.0_v4.3-v4.8.zip) |
| **4.2.x** | [gambio-security-update-2026-09-v1.0_v4.2.zip](https://github.com/gambio/security-patches/releases/download/security-update-2026-09-v1.0/gambio-security-update-2026-09-v1.0_v4.2.zip) |
| **4.0.x – 4.1.x** | [gambio-security-update-2026-09-v1.0_v4.0-v4.1.zip](https://github.com/gambio/security-patches/releases/download/security-update-2026-09-v1.0/gambio-security-update-2026-09-v1.0_v4.0-v4.1.zip) |

Welche Version dein Shop hat, siehst du im Gambio Admin unterhalb der Menüpunkte. Welche
Versionslinien noch Sicherheitsupdates erhalten, steht in der
[Versionsübersicht](https://developers.gambio.de/version-overview/).

## Download prüfen

Du brauchst dafür keine technischen Kenntnisse. Diese drei Punkte reichen:

1. **Lade den Patch nur von dieser Seite herunter.** In der Adresszeile deines Browsers muss
   `github.com/gambio/security-patches` stehen.
2. **Vergleiche den Dateinamen.** Er muss genau so heißen wie in der Tabelle oben.
3. **Vergleiche die Dateigröße.** Jede Datei ist etwa 25 KB groß. Eine deutlich größere oder kleinere
   Datei stammt nicht von hier.

Wenn etwas nicht passt, lösche die Datei und lade sie erneut von dieser Seite herunter.

<details>
<summary><strong>Prüfsumme kontrollieren</strong> (optional, für Agenturen und Administratoren)</summary>

Die Prüfsummen aller Dateien stehen in [`SHA256SUMS.txt`](https://github.com/gambio/security-patches/releases/download/security-update-2026-09-v1.0/SHA256SUMS.txt). Die Prüfsumme steht zusätzlich
in unserer Kunden-E-Mail.

**Windows, ohne Kommandozeile:** Wenn [7-Zip](https://www.7-zip.org/) installiert ist, klicke mit der
rechten Maustaste auf die ZIP-Datei und wähle **7-Zip → CRC SHA → SHA-256**. Der angezeigte Wert
muss mit dem Wert in `SHA256SUMS.txt` übereinstimmen.

**Windows (PowerShell)**

```
Get-FileHash .\gambio-security-patch-<version>.zip -Algorithm SHA256
```

**macOS / Linux (Terminal)**

```
shasum -a 256 -c SHA256SUMS.txt
```

Stimmt der Wert nicht überein, verwende die Datei nicht.

</details>

## Installation

Der Patch besteht nur aus Dateien, die per FTP hochgeladen werden. Es ist kein Datenbank-Update nötig.

1. **Datensicherung** anlegen (Dateien und Datenbank). Eine Anleitung liegt als `DATENSICHERUNG.txt` im ZIP.
2. ZIP-Datei **entpacken**.
3. Den **Inhalt** des Ordners `Security Update 2026-09 v1.0` (nicht den Ordner selbst) per FTP in das
   **Hauptverzeichnis deines Shops** hochladen und vorhandene Dateien überschreiben.

Damit ist die Installation abgeschlossen. Die gleiche Anleitung liegt als `Installationsanleitung.txt`
im ZIP. Allgemeine Hinweise zu FTP-Upload und Datensicherung findest du unter
[developers.gambio.de/installation](https://developers.gambio.de/installation/).

Bitte beachte:

- Erstelle vor dem Einspielen eine **vollständige Datensicherung** (Dateien und Datenbank).
- Verwende nur den Patch, der **zu deiner Shopversion** passt.
- Spiele Sicherheitspatches **so schnell wie möglich** ein.

## Fragen

Dieses Repository ist kein Support-Kanal. Bei Fragen zur Installation wende dich bitte an info@gambio.de.

---

# Gambio Security Patches (English)

[Deutsch](#gambio-security-patches) · **English**

This repository provides security patches for Gambio shop versions for download.
It contains only the patch packages and their release notes, no shop source code.

> **Why here?** We are currently experiencing an outage affecting our customer portal, the forum and the blog. Following suspicious activity on our web server, we shut down the affected hardware in a controlled manner as a precaution. We are carefully checking our systems and will then bring the individual services back online step by step. You can find the current status at any time at [www.gambio.de/status](https://www.gambio.de/status).

## Available patches

**Security Update 2026-09 v1.0** (14 September 2026) closes a vulnerability in the StyleEdit login.
There is one ZIP file per version range. Pick the file that matches your shop version and click the
file name to download it.

| Your shop version | Download |
|---|---|
| **26.04.2 – 26.09.1** | [gambio-security-update-2026-09-v1.0_v26.04.2-v26.09.zip](https://github.com/gambio/security-patches/releases/download/security-update-2026-09-v1.0/gambio-security-update-2026-09-v1.0_v26.04.2-v26.09.zip) |
| **26.04.1** | [gambio-security-update-2026-09-v1.0_v26.04.1.zip](https://github.com/gambio/security-patches/releases/download/security-update-2026-09-v1.0/gambio-security-update-2026-09-v1.0_v26.04.1.zip) |
| **4.9.x, 5.0.x, 5.1.0.0, 26.03.0 – 26.04.0** | [gambio-security-update-2026-09-v1.0_v4.9-v26.04.0.zip](https://github.com/gambio/security-patches/releases/download/security-update-2026-09-v1.0/gambio-security-update-2026-09-v1.0_v4.9-v26.04.0.zip) |
| **4.3.x – 4.8.x** | [gambio-security-update-2026-09-v1.0_v4.3-v4.8.zip](https://github.com/gambio/security-patches/releases/download/security-update-2026-09-v1.0/gambio-security-update-2026-09-v1.0_v4.3-v4.8.zip) |
| **4.2.x** | [gambio-security-update-2026-09-v1.0_v4.2.zip](https://github.com/gambio/security-patches/releases/download/security-update-2026-09-v1.0/gambio-security-update-2026-09-v1.0_v4.2.zip) |
| **4.0.x – 4.1.x** | [gambio-security-update-2026-09-v1.0_v4.0-v4.1.zip](https://github.com/gambio/security-patches/releases/download/security-update-2026-09-v1.0/gambio-security-update-2026-09-v1.0_v4.0-v4.1.zip) |

Your shop's version is shown in the Gambio Admin below the menu items. Which version lines still
receive security updates is listed in the
[Version Overview](https://developers.gambio.de/en/version-overview/).

## Verify the download

No technical knowledge is needed for this. These three points are enough:

1. **Download the patch only from this page.** Your browser's address bar must show
   `github.com/gambio/security-patches`.
2. **Compare the file name.** It must match the name in the table above exactly.
3. **Compare the file size.** Every file is about 25 KB. A file that is much larger or smaller did
   not come from here.

If anything does not match, delete the file and download it again from this page.

<details>
<summary><strong>Check the checksum</strong> (optional, for agencies and administrators)</summary>

The checksums of all files are listed in [`SHA256SUMS.txt`](https://github.com/gambio/security-patches/releases/download/security-update-2026-09-v1.0/SHA256SUMS.txt). The checksum is also given in
our customer email.

**Windows, without a command line:** If [7-Zip](https://www.7-zip.org/) is installed, right-click the
ZIP file and choose **7-Zip → CRC SHA → SHA-256**. The value shown must match the value in
`SHA256SUMS.txt`.

**Windows (PowerShell)**

```
Get-FileHash .\gambio-security-patch-<version>.zip -Algorithm SHA256
```

**macOS / Linux (Terminal)**

```
shasum -a 256 -c SHA256SUMS.txt
```

If the value does not match, do not use the file.

</details>

## Installation

The patch consists only of files that are uploaded via FTP. No database update is needed.

1. Create a **backup** (files and database). Instructions are in `DATENSICHERUNG.txt` inside the ZIP.
2. **Unpack** the ZIP file.
3. Upload the **contents** of the folder `Security Update 2026-09 v1.0` (not the folder itself) via FTP
   into the **root directory of your shop** and overwrite existing files.

That completes the installation. The same instructions are in `Installationsanleitung.txt` inside the
ZIP. General guidance on FTP upload and backups is at
[developers.gambio.de/en/installation](https://developers.gambio.de/en/installation/).

Please note:

- Create a **complete backup** (files and database) before installing.
- Use only the patch that **matches your shop version**.
- Install security patches **as soon as possible**.

## Questions

This repository is not a support channel. For installation questions please contact info@gambio.de.
