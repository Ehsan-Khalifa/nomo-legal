---
title: NoMo — Privacy Policy
---
# NoMo — Privacy Policy

**Last updated: 23 July 2026**

This Privacy Policy explains what personal data the NoMo mobile app ("NoMo", the
"App", "we", "us", "our") collects, why, where it goes, and the choices you have.
NoMo is a personal travel-safety app (location wake-up alarms plus family-safety
features such as live location sharing, emergency contacts, and crash detection).

Because NoMo is a **location and safety app**, most of what it handles is
sensitive by nature. We've tried to collect as little as possible and keep it on
your device wherever we can.

> The App's operator is finalising its formal legal registration. The registered
> entity name and address will be added here once available. Until then, contact
> us at the address in Section 11.

---

## 1. The short version

- You can use core alarm features **without an account** — that data stays on
  your device.
- We do **not** sell your data, show ads, or use advertising/analytics tracking
  SDKs.
- Precise location is central to how NoMo works and is used to power alarms,
  navigation, live sharing, and safety alerts.
- Some data (search text, coordinates, route endpoints) is sent to Google and
  Open-Meteo to return maps, places, routes, and weather.
- You can **permanently delete your account and its data** from within the App.

## 2. Who this applies to

NoMo is intended for users **aged 18 and over**. It is not directed at children,
and we do not knowingly collect data from anyone under 18.

## 3. What data we collect and why

### a. Location data
- **Precise (GPS) location**, including in the background ("always" permission),
  is used to: trigger location/ETA/driving alarms as you approach a destination;
  provide turn-by-turn navigation; show your area, weather, and air quality;
  broadcast your live position during a Live Share session; and attach your
  location to crash and SOS alerts.
- Background location is requested because wake-up alarms must work with the
  screen off and the app in the background.
- Live-session and alarm monitoring uses a foreground service while active.

### b. Account and profile data
- If you sign in, we process your **email address** and a user ID via our
  authentication provider (Supabase), and — if you use Google Sign-In — the
  identity Google returns.
- Optional **display name** and **profile photo** you choose to set.
- You can also use the App in **anonymous mode**, which sets a local flag only
  and creates no server account.

### c. Emergency contacts
- Names and **phone numbers** you save as emergency contacts. These are personal
  data about other people; you should only add contacts who have agreed.
- Used solely to text your live location during a crash alert or SOS.

### d. Places, alarms, and history
- **Saved places** (e.g. Home/Work pins), **alarm definitions**, and your
  **trip and search history** (labels, coordinates, timestamps — up to the most
  recent 200 entries on your device).

### e. Content you share in a session
- During **Live Share**, your name, live coordinates, "arrived" status, SOS flag,
  and any meetup/event details you set are broadcast to the other people in that
  6-digit-code session.

### f. Subscription data
- If you buy NoMo Plus/Pro, purchases are handled by the Google Play Store and
  our billing provider (RevenueCat). **We never receive or store your card, bank,
  or UPI details.** Your account ID is shared with RevenueCat so your
  entitlement follows your account.

### g. Diagnostics
- Technical crash and performance data is sent to Sentry with **personal-data
  scrubbing enabled** (`sendDefaultPii = false`) and only a sample of
  performance traces. We do **not** use analytics or
  advertising SDKs, and we do not build advertising profiles.

## 4. Where your data is stored

| Data | On your device | On our servers (Supabase) |
|---|---|---|
| Alarms, saved places, settings | Yes | Yes, if signed in (backup/sync) |
| Trip/search history | Yes (device storage) | Yes, if signed in |
| Emergency contacts (phone numbers) | Yes, in **secure storage** (Android Keystore / iOS Keychain) | Yes, if signed in (private to you) |
| Profile photo | — | Yes, in file storage, served via a public (unguessable) URL |
| Anonymous-mode flag | Yes | — |

- Server data is protected by **row-level security** so that each user can access
  **only their own** records; a different signed-in user sees none of your data.
- Device backups to the cloud/ADB are disabled for the App so location, contacts,
  and tokens don't leave the device that way.
- Connections to our servers and to third parties use encrypted (TLS) transport.

## 5. Who we share data with (third parties)

NoMo sends data to the following services only to provide the features you use.
Each has its own privacy policy.

| Recipient | What it receives | Purpose |
|---|---|---|
| **Google Maps Platform** (Maps SDK, Places, Routes, Geocoding) | Search text you type, and coordinates (your location bias, route origin/destination/waypoints, points to name) | Maps, place search, navigation, ETA, area labels |
| **Google** (Sign-In) | Your Google identity, if you choose Google sign-in | Authentication |
| **Supabase** | Your account, profile, and the synced data in Section 4 | Auth, database, file storage, real-time Live Share |
| **Open-Meteo** | Your coordinates (no account, no API key) | Weather, UV, air quality |
| **RevenueCat + Google Play Billing** | Your account ID and purchase status | Subscriptions |
| **Sentry** | Technical crash/diagnostic data, PII-scrubbed | Stability monitoring |
| **Your mobile carrier** | The SMS you send (your location link + message) | Delivering safety texts |
| Other **Live Share participants** | Your name, live location, SOS/arrival status | The sharing feature you activated |

We do **not** sell your personal data or share it for advertising.

## 6. Legal bases and consent

- You grant device permissions (location, notifications, alarms, SMS, contacts)
  through the operating system's own prompts; you can change or revoke them at any
  time in your device settings.
- SMS and contacts permissions are requested only when you activate a feature that
  needs them, not at startup.
- Under India's **Digital Personal Data Protection Act, 2023 (DPDP Act)**, we
  process your personal data on the basis of the **consent** you give through
  the operating system's permission prompts and your in-app choices (e.g.
  enabling Live Share, adding an emergency contact), and for the **legitimate
  use** of providing the service you have voluntarily requested.
- You may **withdraw consent at any time** — by disabling the permission in
  device settings, turning the feature off in the App, or deleting your
  account. Withdrawing consent stops future processing, but the dependent
  feature will stop working; withdrawal does not affect processing already
  carried out.
- If you serve EU/UK users in future, GDPR/UK-GDPR sections should be added
  before launch there.

## 7. Retention

- **Device data** stays until you delete it in the App, or uninstall/clear the
  App. History is capped at the most recent 200 entries.
- **Server data** is kept for as long as your account exists and is deleted when
  you delete your account (see Section 8).
- **Crash/diagnostic events** at Sentry are retained for 90 days (Sentry's
  standard retention) and then deleted automatically.

## 8. Your choices and rights

- **Delete your account and data.** In the App: **Profile → Delete account**.
  This cascades on our servers to remove your profile, saved places, alarms,
  history, settings, emergency contacts, and your profile photo, and clears the
  App's data on your device. **Deletion is irreversible.** If you no longer
  have the App installed, request deletion at
  [delete-account.html](delete-account.html) or by emailing us (Section 11)
  from the address on the account.
- **Delete some data without deleting your account.** Saved places, alarms,
  emergency contacts, and fences can each be removed individually inside the
  App; the change syncs to our servers.
- **Sign out** at any time; anonymous-mode and device data can be cleared by
  clearing/uninstalling the App.
- **Manage permissions** (location, notifications, SMS, contacts) in your device
  settings.
- **Manage or cancel subscriptions** via Google Play / the in-app subscription
  screen.
- Under the DPDP Act you have the right to **access** a summary of the personal
  data we process, to have inaccurate or incomplete data **corrected**, to have
  your data **erased** (via in-app account deletion or by request), to an
  accessible **grievance-redressal** mechanism (Section 11), and to **nominate**
  a person to exercise your rights if you are incapacitated. The App does not
  currently offer an automated data **export**; to make an access, correction,
  or portability request, contact us at Section 11 and we will handle it
  manually.

## 9. Security

- Emergency-contact phone numbers are stored in platform secure storage
  (Keystore/Keychain), not plaintext.
- Server records are isolated per user via row-level security.
- App-level lock (device biometric/PIN) is available to gate access to the App.
- Cloud/ADB backup of the App's data is disabled.
- No security measure is perfect; we cannot guarantee absolute security.

## 10. Children

NoMo is not intended for and is not directed to children under 18. If you believe
a minor has provided us data, contact us and we will delete it.

## 11. Contact and grievance redressal

Questions, privacy requests, or grievances: **nomo.dev001@gmail.com**.

For the purposes of India's DPDP Act, this address is our grievance-redressal
contact. We aim to acknowledge grievances promptly and resolve them within a
reasonable period, and in any case within the timelines prescribed by
applicable law. If you are not satisfied with our response, you may complain to
the **Data Protection Board of India**.

## 12. Changes to this policy

We may update this policy. Material changes will be signalled by updating the
"Last updated" date and, where appropriate, an in-app notice.

---

