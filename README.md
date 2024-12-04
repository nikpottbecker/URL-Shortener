# URL Shortener von querf.de

Dies ist der URL-Shortener von **querf.de**, mit dem Nutzer lange URLs auf einfache und benutzerfreundliche kurze Links umwandeln können. Dieser Dienst ermöglicht es, Links zu kürzen, die dann einfach geteilt und erinnert werden können.

## Funktionen

- Kürzen von langen URLs in benutzerfreundliche, kurze Links.
- Möglichkeit, benutzerdefinierte Kürzel zu erstellen.
- Einfache Verwaltung und Generierung von Kurz-URLs.
- Integriertes Tracking der Klicks auf die generierten Kurz-URLs.

## Nutzung

### URL kürzen auf querf.de

1. Besuche die Website [querf.de](https://querf.de).
2. Gib die lange URL in das Eingabefeld ein.
3. Klicke auf "Kürzen".
4. Deine kurze URL wird sofort generiert und ist bereit zur Verwendung.

### Beispiel

Lange URL: `https://www.example.com/long-url-example`
Kürzere URL: `https://querf.de/abcd1234`

## API

Es gibt auch eine API, mit der du URLs automatisch kürzen kannst.

- **POST** `/api/shorten` - Kürzt eine URL und gibt die kurze URL zurück.

**Beispiel:**

```bash
curl -X POST -d "url=https://www.beispiel.com" https://querf.de/api/shorten
