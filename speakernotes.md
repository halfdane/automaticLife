# Automatic Life: vollautomatische Deployments für otto.de

## Otto-Intro
- Vom ersten Katalog über CD zur Website
- Heute mit 12 agilen Teams
- Vertikalen und meine Vertikale
- mehrere Dutzen Livegänge täglich

- Stichpunkte: agil, viele Livegänge, viele automatisierte Tests

- Warum sind viele Livegänge ein Mehrwert?



## MTTF - "Mit ein bisschen Planung hätte man das verhindern können"
- Optimierung "Mean time to failure"
- wie lange dauert es, bis etwas schiefgeht
- es ist teuer, wenn etwas schiefgeht
- alle eventualitäten einplanen:
-- lange, detaillierte Planung
-- intensive, manuelle Testphase
-- viele Nacharbeiten
-- Häuserbau - offensichtliche Schwächen bei Großprojekten
- Anforderungen werden nicht gut verstanden oder ändern sich
- es geht ja trotzdem immer irgendetwas schief

## MTTR - "Wir lösen Probleme, wenn wir sie haben"
- Optimierung "Mean time to recovery"
- Grundannahme ändern: es ist _nicht_ teuer, wenn etwas schiefgeht
-- "if it hurts, do it more often"
-- maximale automatisierung
-- kurze Zyklen -> kurze Planung
-- kurze manuelle Testphase - manchmal gar keine
-- Nacharbeiten sind wie geänderte Anforderungen schnell Verfügbar
- wenn etwas schiefgeht, sind die Korrekturen ebenso schnell am Platz

## Life Coding
- Request-Header (X-EXPERTEN: WERKSTATT) -> CSS-Klasse setzen -> Hintergrundfarbe ändern
- Toggle einbauen und toggeln

- Push
-- Build, Unit- / Komponenten- / Acceptance-Tests für alle commits des Teams -> Continuous Integration
-- Deployment auf CI -> Deployment auf DEV -> Continuous Delivery
-- FOLIE: Blue-Green Deployment
-- FOLIE: CDCs
-- Deployment auf Prelive -> Layouttests -> Deployment Live -> Smoketests -> Continuous Deployment

## Testabdeckung
- Vertrauen
- Geschwindigkeit
- Zero-Bug-Policy
