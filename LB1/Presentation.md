# Presentation Software- und Datenintegritätsfehler

## Was ist das Problem

Wenn Daten über das internet übertragen werden könnten diese unterwegs von dritten verändert werden. Dies gilt es zu vermeiden.

## Man kann unterscheiden zwischen Softwareintegrität und Datenintegrität

### Softwareintegrität

Software wie Programme oder Betriebssysteme welche aus dem Internet heruntergeladen werden.

### Datenintegrität

Allgemeine Daten welche im Internet herumgeschickt werden. z.B. Nachrichten.

## Warum ist das wichtig?

- Installation von modifizierter Software verhindern
- Verändern von Daten verhindern

## Datenintegrität -> PGP-Verschlüsselung

Der Absender verschlüsselt die Nachricht mit public Key.

Der Empfänger entschlüsselt die Nachricht dann mit private key.

## Beispiel Checksumme

1. File Downloaden -> `DownloadedFile.exe`
2. Checksum generieren (Powershell)

```powershell
certutil -hashfile "DownloadedFile.exe" md5
# or
certutil -hashfile "DownloadedFile.exe" sha1
# or
certutil -hashfile "DownloadedFile.exe" sha256
# or
certutil -hashfile "DownloadedFile.exe" sha384
# or
certutil -hashfile "DownloadedFile.exe" sha512
```

3. Checksum mit herstellerwebseite vergleichen.
