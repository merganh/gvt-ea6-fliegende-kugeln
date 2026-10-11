# EA 6: Objekte bewegen, fliegende Kugeln

Einsendeaufgabe 6, Modul Graphical Visualisation Technologies, TH Lübeck, Wintersemester 2026/27.

Eine einseitige WebGL-Anwendung (rohes WebGL 1, keine Bibliothek). Ein Torus und vier Kugeln
stehen über einer Ebene aus Gitterlinien. Die vier Kugeln fliegen kontinuierlich auf Kreisbahnen
durch das Loch des Torus und berühren weder einander noch den Torus. Mit der Taste `k` wird die
Bewegung ein- und ausgeschaltet. Als Erweiterung dreht sich der Torus zusätzlich um eine gekippte
Achse in seiner Ringebene, synchron zur Kugelbewegung.

## Live-Demo

Öffentlich erreichbar unter:
<https://merganh.github.io/gvt-ea6-fliegende-kugeln/>

## Lokal ausführen

Kein Build-Schritt. Die Seite lässt sich über einen lokalen Server öffnen:

```bash
python3 -m http.server 8000
# dann im Browser: http://localhost:8000
```

## Deployment via GitHub Pages

Im Repo liegt ein Workflow unter `.github/workflows/pages.yml`, der die Seite bei
jedem Push auf `main` automatisch nach GitHub Pages deployt. Einmalig im Repo
unter **Settings → Pages → Build and deployment → Source** `GitHub Actions`
wählen.

## Aufbau

- `index.html`: gesamte Anwendung in einer Datei (HTML, CSS, JS inline), eigene Matrixfunktionen, keine externen Bibliotheken

## Bedienung

- **k**: automatische Bewegung ein- bzw. ausschalten

Es gibt einen gleichnamigen Button. Beim Ausschalten bleiben alle Objekte stehen, beim Einschalten läuft die Bewegung ohne Sprung weiter.

## Quelltext-Markierung

Die für die Aufgabe geschriebenen JavaScript-Stellen sind mit
`// START EA6_FLIEGENDE_KUGELN` und `// END EA6_FLIEGENDE_KUGELN` markiert.
