# Ranglisten-Website

## Dateien

- `index.html` – komplette Website
- `data.json` – Nutzer, Punkte und Ranglisten-Konfiguration

## Daten ändern

In `data.json` können Nutzer ergänzt oder Punkte geändert werden:

```json
{
  "users": [
    { "username": "Spieler", "points": 12345 }
  ]
}
```

Neue Tabs werden ebenfalls über `leaderboards` angelegt. Für `icon` können Lucide-Icon-Namen verwendet werden.

Die Profilbilder werden automatisch über
`https://render.crafty.gg/2d/head/USERNAME?size=256`
geladen.
