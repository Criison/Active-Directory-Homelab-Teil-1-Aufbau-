# Screenshot-Übersicht

Alle Bilder liegen in `screenshots/`. ⭐ = wird in der README angezeigt.

| Datei | Abschnitt | Was zu sehen ist |
|---|---|---|
| ⭐ 01-proxmox-uebersicht.png | 1 Umgebung | Proxmox: alle VMs/Container, Auslastung, Speicher |
| ⭐ 02-rdp-fehler-0x204.png | 3 RDP | Fehler 0x204 – Port 3389 nicht erreichbar |
| 03-ausgangslage-gpo-azubi-sperren.png | 2 Ausgangslage | Alte Azubi-GPO: Sperre + Laufwerk Z: per IP, gilt für alle |
| ⭐ 04-ou-gruppen.png | 5 Gruppen | OU Gruppen mit GG-IT, GG-Buchhaltung, GG-Azubis, IT-Administratoren |
| ⭐ 05-testuser-gruppen.png | 9 Aufräumen | Test User nur noch in Domänen-Benutzer + GG-Buchhaltung |
| ⭐ 06-effektiver-zugriff-jdoe.png | 6 Freigabe | John Doe: Rechte „Ändern“ auf IT-Daten |
| ⭐ 07-effektiver-zugriff-tu.png | 6 Freigabe | Test User: kein Zugriff, eingeschränkt durch Dateiberechtigungen |
| ⭐ 08-client-zugriff-verweigert.png | 6 Freigabe | Client: Z: sichtbar, Zugriff verweigert (Stand vor der GPO-Aufteilung) |
| ⭐ 09-gpo-laufwerk-z.png | 7 GPOs | Neue GPO: Z: → \\DCTEST\IT-Daten |
| 10-filter-laufwerk-gg-it.png | 7 GPOs | Sicherheitsfilterung Laufwerks-GPO → GG-IT |
| ⭐ 11-filter-azubi-gg-azubis.png | 7 GPOs | Sicherheitsfilterung Azubi-GPO → GG-Azubis |
| ⭐ 12-test-jdoe-mit-z.png | 7 GPOs | John Doe am Client: Z: vorhanden |
| ⭐ 13-test-azubi-ohne-z.png | 7 GPOs | Leon Mueller am Client: kein Z: |
| 14-kennwortrichtlinien.png | 8 Kennwort | Kennwortregeln der Default Domain Policy |
| ⭐ 15-kontosperrung.png | 8 Kennwort | Kontosperrung 5 Versuche / 15 Min / 15 Min |
| ⭐ 16-konto-gesperrt-client.png | 8 Kennwort | Anmeldemeldung „Konto gesperrt“ |
| ⭐ 17-kontosperre-aufheben-ad.png | 8 Kennwort | AD: Option „Kontosperrung aufheben“ |
| 18-gpo-doublette.png | 9 Aufräumen | Nicht verknüpfte GPO mit doppelter Einstellung |
| 19-snapshots.png | 10 Backups | Snapshot-Kette des Clients |
| 20-backup-dc.png | 10 Backups | Backup DC (14,7 GB) |
| ⭐ 21-backup-client.png | 10 Backups | Backup Client (18,2 GB) |
| ⭐ 22-fehler-falscher-ordner.png | 12 Fehler | Rechte von C:\ statt C:\IT-Daten geöffnet |
| 23-fehler-nur-lesen.png | 12 Fehler | GG-IT zunächst nur mit „Lesen, Ausführen“ |
| 24-test-buchhaltung-ohne-z.png | 7 GPOs | Test User am Client: kein Z: |
| 25-gpupdate-client.png | 4 OU | gpupdate /force am Client, Z: kommt an |
| 26-ntfs-vorher.png | 6 Freigabe | NTFS-Rechte vor dem Aufräumen (Benutzer, unbekannte SID) |
| 27-ad-benutzer.png | 1 Umgebung | Benutzer in der OU Benutzer |
| 28-kerberos.png | 8 Kennwort | Kerberos-Richtlinie (5 Min Zeittoleranz) |

## Noch nachzureichen (optional)
- NTFS-Liste von IT-Daten im **Endzustand** (GG-IT mit „Ändern“) → Abschnitt 6
- Reiter **Delegierung** einer gefilterten GPO (Authentifizierte Benutzer: Lesen) → Abschnitt 7
- Leon Mueller: Sperrmeldung bei `control` → Abschnitt 7
