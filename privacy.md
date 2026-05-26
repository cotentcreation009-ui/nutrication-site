---
title: Privacy Policy
layout: default
permalink: /privacy/
---

# Nutrication Privacy Policy

**Last updated:** May 25, 2026

Nutrication is built around a simple promise: the data you give us should only
be used to make your scans more useful to *you*. This page explains exactly
what we collect, where it goes, and how to delete it.

If something here isn't clear, email us: **support@nutrication.app**.

---

## What we collect

### On your device only (never sent to our servers)
- **Your profile** — name, demographics, health concerns, allergens, diet
  preferences, cooking preferences, goals, daily nutrient targets, family
  history, medications, personal notes. Stored in your device's local app
  storage. We never sync this anywhere unless you explicitly sign in.
- **Saved restaurant menus** — when you tap "Save this menu" the scored
  payload is kept in local app storage so you don't have to re-scan.
- **Day notes and events** — calendar notes and planned events you add
  through the Calendar tab.

### Stored on our servers
- **Scan history** — barcode, label-photo, meal-photo, menu-photo, and
  recipe scans you create. We keep the scored result plus a reference to
  the food/product so the History tab and "Eat again" row work. Tied to
  either your account (if you signed in) or a randomly-generated device ID.
- **Calendar entries** — what you logged you ate and when, the macros, and
  the slot (breakfast/lunch/dinner/snack). Same identity tie as above.
- **Cached scoring results** — once we score a product or analyze a menu,
  we keep the result for up to 30 days so re-opening the same scan is
  instant.

### Sent to AI vendors for processing
- **Photos** — when you scan a label, meal, or menu, the image is sent to
  Google Gemini for content recognition (food items, portions, macros,
  ingredient parsing). Per Google's terms, these images are not used to
  train Gemini and are deleted from Google's processing pipeline after
  the request completes.
- **Dish names + macros** — when you customize a menu item before logging,
  the dish name and per-serving macros are sent to Gemini for component
  decomposition. No identifying information accompanies these requests.

### Sent to other infrastructure
- **Supabase** (auth + database): if you sign in with email, your email
  address is held by Supabase under their security policies. Scan history
  and calendar entries are stored in Supabase Postgres.
- **Upstash Redis**: short-term cache of scoring results. No personal
  information.
- **Open Food Facts**: barcode lookups query the public Open Food Facts
  database. The barcode is sent; no personal info accompanies it.
- **Sentry**: when an unexpected error happens in the app, the stack trace
  and basic device info (model, iOS version, app version) are sent to
  Sentry so we can fix bugs. No scan content, photos, or profile data
  are included. If you'd rather opt out, see "Opt out of crash reporting"
  below.

### What we don't collect
- We do not track you across apps or websites.
- We do not sell your data to anyone, ever.
- We do not show ads.
- We do not share data with insurance, marketing, or analytics brokers.
- We do not use HealthKit unless you explicitly opt in (we currently don't
  integrate HealthKit at all).

---

## Permissions we request

| Permission | What it's for |
| --- | --- |
| **Camera** | Scan barcodes, photograph nutrition labels, photograph meals, photograph restaurant menus. Only invoked when you tap a scan action. |
| **Photo library** | Pick an existing photo of a label, meal, or menu to scan instead of taking a new one. |

We don't access either until you tap a scan action. We don't request
location, contacts, microphone, or any background permissions.

---

## How long we keep it

| Data | Retention |
| --- | --- |
| Scan history (server) | Until you delete it or your account, whichever comes first |
| Profile (device) | Until you uninstall the app or clear it from the You tab |
| Calendar entries (device) | Until you delete them or uninstall |
| Cached scoring results | Up to 30 days, then automatically expired |
| Account email (Supabase) | Until you delete your account |
| Crash reports (Sentry) | 30 days, then automatically expired |

---

## Deleting your data

You have two paths:

1. **Delete a single scan, day, or menu** — tap into it and choose Delete.
2. **Delete your entire account and all server-side data** — open the You
   tab, scroll to "Account", tap **Delete my account & data**. This permanently
   removes your scan history, calendar entries, account email, and
   on-device data. There's no recovery after this.

If you can't reach the in-app delete (e.g. you lost device access), email
**support@nutrication.app** and we'll remove your data within 30 days
of receiving a verified request.

---

## Opt out of crash reporting

Crash reports are anonymous and contain no scan content, but if you'd
prefer to disable them entirely, email **support@nutrication.app** and
we'll send you a build with crash reporting compiled out.

---

## Children

Nutrication is not directed to children under 13. If you become aware that a
child under 13 has signed up, contact us and we'll delete the account
within 7 days.

---

## Changes to this policy

If we change what we collect or how we use it, we'll update this page and
push a notification in the app the next time you open it. We won't change
the policy in a way that materially expands data collection without your
explicit re-consent.

---

## Contact

Privacy questions: **support@nutrication.app**
Support: **support@nutrication.app**
