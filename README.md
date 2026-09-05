# Legal Scan Pro

Build a Legal Metrology Compliance Checker web app for scanning packaged

commodity labels against India's Legal Metrology (Packaged Commodities)

Rules, 2011.

Set up Supabase auth with three user roles: inspector, manufacturer, admin.

Screens needed:

1. Login/signup screen (role selection on signup)

2. Upload screen — user can upload one or more photos of a product label

   (supports multiple photos per single "scan")

3. Results screen — shows extracted label fields (manufacturer name/address,

   country of origin, commodity name, net quantity, mfg date, best-before

   date, MRP, consumer care details, unit sale price) and a compliance

   status (compliant / non-compliant / exempt) with a list of any violations

   found, each showing severity (critical/minor) and the rule it violates

4. History screen — a searchable list of past scans, filterable by product

   name, manufacturer, date range, and compliance status

Use a clean, professional dashboard style suited to government/enforcement

use — not a consumer app aesthetic.

Set up the Supabase backend with tables for: users (with role), products,

scans, evidence_photos (multiple photos per scan), extracted_fields,

violations, and reports. Don't worry about the exact schema yet — I'll

provide the full SQL after this initial build.

This project was built with [Lovable](https://lovable.dev).

**Live app**: https://compli-checker-pro.lovable.app

## Build with Lovable

Continue developing this project in the [Lovable editor](https://lovable.dev/projects/cc60e273-ceb3-4cec-b200-e797aabd7bfc).

- **Ship faster**: describe what you want to build and Lovable handles the code.
- **Stay in sync**: every change made in Lovable is committed straight to this repository.
- **Full ownership**: this code is yours. Push to `main` on GitHub and your changes sync back into Lovable, ready for your next prompt.

## Development

Prefer working locally? You need Node.js and npm — [install with nvm](https://github.com/nvm-sh/nvm#installing-and-updating).

```sh
git clone <this-repository-url>
cd <repository-name>
npm i
npm run dev
```
