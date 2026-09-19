# GADIT v2.6 — Sync API + SQLite/Drift

Pacchetto autonomo di integrazione per GADIT v2.6.
Include lo schema SQLite/Drift lato Flutter e il modulo API di sincronizzazione lato backend.

## Client
- Drift/SQLite locale
- record operativi
- coda offline
- idempotency key
- push/pull incrementale
- conflitti HTTP 409

## Backend
- POST /sync/records
- GET /sync/records
- tabelle PostgreSQL per idempotenza e conflitti

Prima della compilazione Flutter:
dart pub get
dart run build_runner build --delete-conflicting-outputs

Il modulo backend va collegato ai servizi JWT/database della base GADIT v2.5/v2.6 esistente.
