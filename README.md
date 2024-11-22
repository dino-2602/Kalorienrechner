# Kalorienrechner mit Dark Mode und PAL-Faktoren

Dieses Projekt enthält eine PHP-Anwendung zur Berechnung des täglichen Kalorienbedarfs basierend auf Geschlecht, Alter, Gewicht, Größe und PAL-Faktoren. Es wurde besonderer Wert auf Benutzerfreundlichkeit gelegt, einschließlich eines **Dark Mode** mit Speicherfunktion.

## Projektstruktur

- **`kalorienrechner.php`**: Hauptdatei, enthält die gesamte Logik und Darstellung.
- **`style.css`**: Individuelle CSS-Stile zur Anpassung des Designs.
- **`bootstrap.min.css`**: Bootstrap-Stylesheet für responsives Layout und Grunddesign.

## Funktionen

1. **Berechnung des Kalorienbedarfs**:
   - Basierend auf Geschlecht, Alter, Gewicht und Größe.
   - Einbeziehung von PAL-Faktoren (Schlafen, Sitzen, Stehen, Sport, Sonstige).
   - Begrenzung der PAL-Faktoren auf maximal **24 Stunden Gesamtzeit**.

2. **Dark Mode mit Speicherfunktion**:
   - Umschalten zwischen Light Mode und Dark Mode über einen Switch-Button.
   - Zustand wird mit **localStorage** gespeichert und beim Laden der Seite wiederhergestellt.

3. **Fehlervalidierung**:
   - Alle Eingabefelder müssen ausgefüllt werden.
   - Keine negativen oder Null-Werte erlaubt.
   - Gesamtzeit der PAL-Faktoren darf nicht über **24 Stunden** liegen.

## Installation und Ausführung

1. **Bootstrap und CSS einrichten**:
   - Lade Bootstrap herunter und speichere es im Ordner `bootstrap/css`.
   - Stelle sicher, dass deine `style.css` im Ordner `css` liegt.

2. **Projektdatei speichern**:
   - Speichere die Datei `kalorienrechner.php` im entsprechenden Verzeichnis deines Webservers (z. B. `htdocs` bei XAMPP).

3. **Webserver starten**:
   - Starte den Apache-Server über XAMPP.

4. **Seite im Browser öffnen**:
   - Rufe die Datei auf: `http://localhost/<Pfad-zum-Projekt>/kalorienrechner.php`.

## Eingabefelder

- **Geschlecht**: Auswahl zwischen Männlich und Weiblich.
- **Alter**: Positive Ganzzahl (ab 1 Jahr).
- **Gewicht**: Positive Zahl in Kilogramm.
- **Größe**: Positive Zahl in Zentimetern.
- **PAL-Faktoren**:
  - **Schlafen (Std)**: Stunden pro Tag.
  - **Sitzen (Std)**: Stunden pro Tag.
  - **Stehen (Std)**: Stunden pro Tag.
  - **Sport (Std)**: Stunden pro Tag.
  - **Sonstige (Std)**: Stunden pro Tag.

## Fehlermeldungen

- **Alter, Gewicht, Größe**:
  - Wert darf nicht leer, negativ oder 0 sein.
- **PAL-Faktoren**:
  - Keine negativen oder leeren Werte erlaubt.
  - Gesamtzeit darf maximal **24 Stunden** betragen.

## Technologien

Hier sind die verwendeten Technologien in diesem Projekt:

- [![PHP](https://img.shields.io/badge/PHP-%23777BB4.svg?&style=for-the-badge&logo=php&logoColor=white)](https://www.php.net/)
- [![JavaScript](https://img.shields.io/badge/JavaScript-%23F7DF1E.svg?&style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
- [![Bootstrap](https://img.shields.io/badge/Bootstrap-%23563D7C.svg?&style=for-the-badge&logo=bootstrap&logoColor=white)](https://getbootstrap.com/)
- [![CSS](https://img.shields.io/badge/CSS3-%231572B6.svg?&style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)

## Screenshot

![Kalorienrechner](https://github.com/dino-2602/Kalorienrechner/blob/main/Kalorienrechner/screenshots/Kalorienbedarf%20berechnen.png)

## Lizenz

Dieses Projekt ist für Bildungszwecke im Rahmen des ITL-Unterrichts an der Landesberufsschule Eibiswald gedacht.
