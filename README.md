### Jalaram Feeds

Cattle feed production group. Humne apna poora digital setup khud banaya hai —
Cloudflare Workers + D1 par chalne wala custom ERP, bina kisi heavy framework
ke, sab kuch WhatsApp automation ke saath joda hua.

## Systems

- **ERP** — Sales, Purchase, Production, Labour, Lab aur Gate (login, reports,
  stock/ledger, Day End, EA modules, approvals) — sab alag-alag Workers me,
  ek hi gate ke peeche
- **HR module** — Employee Master, roz ki hazari (attendance), chhutti
  (approval flow), advance aur mahine ki tankhwah
- **Truck Tracker** — live gadi tracking, trip km, odometer, diesel aur kharcha
  ka hisab; driver ke liye Android (Kotlin) app, server par Worker + D1
- **Tally integration** — Tally se sirf-padhne-wala data pull (read-only export)
  karke D1 me load, aur us data ko web par dekhne wala viewer
- **Meeting manager** — departments ke recurring meetings, WhatsApp reminders,
  MOM (Minutes of Meeting) PDF ke saath
- **Payroll/Attendance dashboard** — PagarBook ke data se attendance aur salary
  sheet (company-wise formats ke saath)
- **WhatsApp automation** — reports, alerts, reminders aur approvals sab
  WhatsApp par

## Tech stack

Cloudflare Workers · D1 (SQLite) · R2 · Cron Triggers · Vanilla JS
(koi framework nahi) · Kotlin (driver app) · Python (Tally sync scripts)

## Repos

Public: `jf` (purana static dashboard, ab archive) · `Jalaramfeeds` (ye profile)
Baaki production repos private hai — code, databases aur live URLs safe rakhe hai.
