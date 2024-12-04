# URL Shortener für querf.de

Dies ist der URL-Shortener für die Domain **querf.de**, der es ermöglicht, lange URLs auf eine kürzere und einfach zu merkende Form zu kürzen. Dieses Projekt dient als Teil der Webinfrastruktur von QUERF und ist eine einfache und effiziente Lösung zum Teilen von Links.

## Funktionen

- Kürzen von langen URLs in benutzerfreundliche kurze Links.
- Möglichkeit zur Verwaltung und Anpassung von Kurz-URLs.
- Tracking der Klicks auf die kurzen Links.

## Installation

### Voraussetzungen

- **PHP 7.4+**
- **MySQL** oder eine kompatible Datenbank
- **Apache** oder **Nginx** Webserver
- Composer

### Schritt-für-Schritt-Anleitung

1. **Clone das Repository**:
    ```bash
    git clone https://github.com/nikpottbecker/URL-Shortener.git
    cd URL-Shortener
    ```

2. **Installiere die Abhängigkeiten**:
    ```bash
    composer install
    ```

3. **Erstelle die Datenbank und die Tabellen**:
    Erstelle eine MySQL-Datenbank und führe das SQL-Skript aus, das im `database` Ordner enthalten ist, um die notwendigen Tabellen zu erstellen.

4. **Konfiguriere die Verbindung zur Datenbank**:
    Bearbeite die Datei `.env` und stelle sicher, dass die Datenbankverbindungsdetails korrekt sind.

5. **Starte den Webserver**:
    Stelle sicher, dass der Webserver so konfiguriert ist, dass er auf das Projekt zeigt und die URLs richtig verarbeitet werden.

## Nutzung

- Gehe zu `http://deinedomain.com/shorten`, um eine URL zu kürzen.
- Gib die lange URL ein und klicke auf "Kürzen".
- Deine kurze URL wird dir angezeigt und kann sofort verwendet werden.

## API

Es gibt eine API für den URL-Shortener, die Folgendes ermöglicht:

- **POST** `/api/shorten` - Kürzt eine URL und gibt die kurze URL zurück.

**Beispiel:**

```bash
curl -X POST -d "url=https://www.beispiel.com" http://deinedomain.com/api/shorten
