# Changelog — ORY Akademie Landingpage

Domain: https://akademie.ory-berlin.de · Deploy: `npx vercel deploy --prod --yes` (Git-Push deployt nicht automatisch)

## 2026-06-12 — Dynamik & medizinische Seriosität (`78c484d`)

### Dynamische Elemente
- **Hero-Shrink:** „Medizin, die die Ursache behandelt" startet groß und schrumpft beim Scrollen (scale 1 → 0.82 + Opacity-Fade, Badge/Untertitel faden mit)
- **Scroll-Reveal:** Alle Karten und Sektionen (Seminare, E4, Team, Testimonials, FAQ, Steps) gleiten gestaffelt von unten ein (IntersectionObserver, 70ms Versatz pro Element)
- **Scroll-Fortschrittsbalken:** 3px Gradient-Linie (#A8E8E2 → #889FFE) am oberen Rand
- **Kompakte Nav beim Scrollen:** 62px → 54px mit Schatten
- **Nav-Anker mit Scrollspy:** Ansatz · Seminare · Qualität · FAQ (sichtbar ab 1180px), aktiver Abschnitt mit Gradient-Unterstrich
- **Zahlen-Leiste mit Count-up:** 5 Seminarmodule · 4 Säulen (E4) · 3 Ebenen · 2 Formate — nur belegbare Fakten (HWG-konform)

### Neue Sektion `#qualitaet` — „Wissenschaftlicher Anspruch"
Vier Prinzipien für medizinische Seriosität:
1. Evidenzorientierte Inhalte (aktuelle Fachliteratur, laufend aktualisiert)
2. Sicherheit zuerst (Indikationen, Kontraindikationen, Hygiene, Notfallmanagement als Pflichtteil)
3. Dokumentierte Curricula (Lehrpläne, Kursmaterial, Teilnahmebestätigung, BCHT-Anerkennung)
4. Kleine Gruppen, echte Praxis (supervidierte Übungen)

### Barrierefreiheit
- `prefers-reduced-motion` wird respektiert (CSS + JS): alle Animationen aus, Inhalte sofort sichtbar

### Offen / Nächste Schritte
- Echte Dozenten-Profile mit Fotos (User legt Bilder-Ordner an)
- Literaturhinweise pro Modul, Beispiel-Curriculum als PDF, BCHT-Fortbildungspunkte konkret benennen
