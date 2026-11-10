# Webseite online stellen – clevercapsule.de (kostenlos, ca. 20 Minuten)

Die Datei `CNAME` (Inhalt: `clevercapsule.de`) mit hochladen. Sie sagt GitHub, unter welcher Domain die Seite läuft.

Diese Webseite enthält Startseite, Impressum, Datenschutzerklärung, Nutzungsbedingungen, Support und `app-ads.txt`.
Sie besteht nur aus fertigen Dateien. Es gibt keinen Server, keine Datenbank und keine Cookies.

> **Vorher:** Alle gelb markierten Platzhalter (Name, Anschrift, E-Mail) müssen ausgefüllt sein. Schick mir die Angaben,
> dann baue ich die Seite neu. Oder du trägst sie oben in `build.py` ein und führst `python3 build.py` aus.

## Variante A: GitHub Pages (empfohlen)

1. Auf **github.com** ein kostenloses Konto anlegen. Der Benutzername steckt später in der Adresse, z. B. `clevercapsule`.
2. Oben rechts **+ → New repository** wählen.
   - **Repository name:** genau `BENUTZERNAME.github.io` (z. B. `clevercapsule.github.io`)
   - **Public** auswählen und **Create repository** klicken.
3. Auf der neuen Seite **„uploading an existing file“** anklicken. **Alle Dateien und den Ordner `img`** aus diesem Ordner
   per Drag & Drop hineinziehen (nicht den übergeordneten Ordner, sondern seinen Inhalt). Danach **Commit changes**.
4. Nach 1–2 Minuten ist die Seite live unter **`https://BENUTZERNAME.github.io/`**.
5. Kontrolle: `https://BENUTZERNAME.github.io/app-ads.txt` muss die AdMob-Zeile anzeigen.

**Änderungen später:** Datei im Repository anklicken → Stift-Symbol → bearbeiten → *Commit changes*.

## Variante B: Netlify Drop

app.netlify.com/drop öffnen und den Ordner hineinziehen. Fertig. Für eine dauerhafte Seite ein kostenloses Konto anlegen.
Bei dieser Variante im Abschnitt „6. Diese Website“ der Datenschutzerklärung den Hoster auf Netlify ändern
(`build.py` → `host`).

## Eigene Domain (optional, ca. 1 €/Monat)

Mit einer eigenen Domain wie `clevercapsule.de` wirkt der Auftritt professioneller. Die Support-E-Mail lautet dann z. B.
`support@clevercapsule.de`. Bei GitHub: *Repository → Settings → Pages → Custom domain*. Die Anleitung des Domain-Anbieters
für „GitHub Pages“ befolgen.

## Wo die Adressen eingetragen werden

| Wo | Was eintragen |
|---|---|
| App Store Connect → App-Informationen → **Datenschutzrichtlinien-URL** | `https://…/datenschutz.html` |
| App Store Connect → Version → **Support-URL** | `https://…/#support` |
| App Store Connect → Version → **Marketing-URL** | `https://…/` (wichtig für `app-ads.txt`) |
| App Store Connect → App-Informationen → **Lizenzvereinbarung** | Standard-EULA von Apple lassen. Die eigenen Nutzungsbedingungen ergänzen sie. |
| AdMob → Datenschutz und Mitteilungen → DSGVO-Mitteilung → **Datenschutz-URL** | `https://…/datenschutz.html` |
| Im Spiel (`www/index.html`, ganz oben bei `LEGAL_BASE`) | `https://…/`. Dann erscheinen in den Einstellungen die Links IMPRINT · PRIVACY POLICY · TERMS. Apple verlangt einen Datenschutz-Link in der App. |

Kurz-Adressen für englische Nutzer: `/privacy.html` und `/terms.html` leiten auf die englischen Abschnitte weiter.

## Hinweis

Die Texte sind sorgfältig erstellte Vorlagen für ein kostenloses Spiel mit AdMob und In-App-Käufen. Sie ersetzen aber keine
Rechtsberatung. Wenn du sichergehen willst, lass sie einmal prüfen, z. B. über einen Rechtstext-Generator mit
Update-Service oder einen Anwalt. Für das Impressum gilt: Ein reines Postfach reicht in Deutschland in der Regel nicht als
„ladungsfähige Anschrift“.
