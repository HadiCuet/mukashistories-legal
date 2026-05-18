# Mukashi Stories — Privacy Policy

**Effective date:** May 4, 2026

This policy explains what data Mukashi Stories collects, why, and the choices you have. Mukashi Stories is a reading app made for children, so this policy is written in plain English on purpose — parents and guardians should be able to read it in a few minutes.

---

## 1. Who we are

Mukashi Stories is an iOS app for reading bilingual children's folk tales — a side-by-side reader where each line shows the source language and the reader's native language together. It is developed and operated by **Abdullah Al Hadi** ("we", "us"). For the purposes of the EU / UK / EEA General Data Protection Regulation (GDPR) and the California Consumer Privacy Act (CCPA/CPRA), Abdullah Al Hadi is the **data controller** for personal data collected through the Mukashi Stories app. For any privacy questions, contact us at **mukashi.dev@gmail.com**.

This policy covers the Mukashi Stories iOS app (also published for iPadOS, macOS, and visionOS).

---

## 2. Data we collect

### Stays only on your device — never sent anywhere

Everything below is stored locally on your device using Apple's SwiftData framework. If you have iCloud Backup enabled, Apple includes this data in your encrypted iCloud backup — that backup is between you and Apple; we have no access to it.

- **Reading progress** — which page of which story you've reached, and which stories you've completed.
- **Saved words** — words you've tapped and saved to "My Words" for later review, plus your spaced-repetition review history.
- **Preferences** — your settings (language pair, theme, font size, layout style, narration preferences, App Lock on/off, parental PIN hash, etc.), stored in iOS user defaults and SwiftData.
- **Daily reading minutes** — used by the parental "daily reading limit" feature. Counted on-device, not sent anywhere.

A parent or guardian can clear any of this at any time from **Parents → Reset Reading Progress / Clear Saved Words / Reset Onboarding**. Uninstalling the app removes all of it.

### Sent to Firebase (Google)

We use two Firebase services from Google to improve the app: **Analytics** and **Crashlytics**. Both are configured for the strictest privacy settings appropriate for a children's app — no advertising identifiers used for personalization, no cross-app tracking, no ads.

**Firebase Analytics** collects:

- A device identifier scoped to this app only (a Firebase installation ID). It cannot identify the reader across other apps.
- Device type, OS version, app version, language, and country (derived from IP).
- Which screens the reader views in the app (Library, Reader, Treasures, Settings, etc.).
- Aggregate feature usage so we can decide what to keep, fix, or build next:
  - Story interactions: which stories are opened, completed, or favorited (story IDs only) — we never send the story text or your translations.
  - Word interactions: that a word was tapped, saved, unsaved, or pronounced. We do log the word itself and its part of speech, because that's how we know which vocabulary kids find useful — we never log who tapped it.
  - Reading session length (in seconds), page-turn direction, and TTS play/pause counts.
  - Spaced-repetition review session results (how many words got, how many missed) — counts only.
  - Settings changes (theme, language pair, layout style, etc.) — names and new values only.
  - Tab switches between Library, Treasures, Parents, and Settings.

**We do NOT request App Tracking Transparency permission.** Ad personalization, ad-related data storage, and ad-user-data sharing are explicitly disabled in the app's `Info.plist` (`GOOGLE_ANALYTICS_DEFAULT_ALLOW_AD_PERSONALIZATION_SIGNALS=false`, `GOOGLE_ANALYTICS_DEFAULT_ALLOW_AD_STORAGE=false`, `GOOGLE_ANALYTICS_DEFAULT_ALLOW_AD_USER_DATA=false`). Your child's IDFA is never read.

**We never call `setUserID()`.** There is no account, no login, and no persistent identity tied to your child across devices.

**What we do NOT send:** the contents of any story, full sentences from the reader, translations the child reads, search queries, photo library content, microphone input, contact info, payment info, location, or any name or personal identifier you or your child enters anywhere. The app does not have a microphone, camera, or photo library permission at all.

### In-app purchases

Mukashi Stories offers an optional **Mukashi Premium** subscription and a one-time lifetime unlock through Apple's standard In-App Purchase system. We use Apple's StoreKit 2 framework to handle the entire purchase flow.

- **Apple processes the payment.** Your payment method (credit card, Apple Cash, etc.) is never seen by the app or by us. Apple charges your Apple ID directly.
- **What the app stores locally:** which product you purchased and your current subscription status. This is what powers the "Premium unlocked" state on this device.
- **What we send to Firebase Analytics:** non-financial purchase events only — for example, *that* a paywall was shown, *that* a purchase started, *that* a purchase completed, the product identifier (e.g. "monthly", "yearly", "lifetime"), and a generic failure reason if a purchase failed. We never send prices, transaction IDs, receipt data, or any payment information to Firebase.
- **Restoring purchases.** If you reinstall the app or sign in on a new device, **Settings → Restore Purchases** asks Apple's servers (not ours) which products are tied to your Apple ID and re-unlocks the appropriate features. We don't keep our own purchase database — Apple is the source of truth.

**Firebase Crashlytics** collects data only when the app crashes or reports a non-fatal error:

- Stack traces from the crash.
- A snapshot of device state at the time of the crash (OS version, device model, memory pressure, etc.).
- Breadcrumbs — short text messages we log as the app runs (e.g. "opened Reader") to help us reproduce the crash. These never contain the words you've saved, story content, or any personal content.
- Non-fatal errors explicitly reported by the app.

---

## 3. Permissions the app asks for

- **Face ID / Touch ID / passcode** — optional, only used when **App Lock** or **biometrics for the Parent Dashboard** are enabled. The check happens locally via Apple's LocalAuthentication framework. Biometric data never leaves the device and is never seen by the app.
- **Notifications** — optional, only when you opt in to a daily reading reminder. Used to send one local reminder at the time you choose. Not used for marketing.

The app does **not** request access to the camera, microphone, photo library, contacts, location, or motion data.

---

## 4. How we use this data

- **Local data** (reading progress, saved words, settings) powers the app's features for the reader — picking up where they left off, reviewing saved words, applying their preferences. It is not used for anything else.
- **Firebase Analytics** tells us which features are actually being used — which stories engage children, which words they save, which layout style they prefer. We look at aggregate counts, not at individual users. The goal is to decide what to improve and what to remove.
- **Firebase Crashlytics** tells us when and why the app crashes so we can fix the underlying bug.

We do not sell your or your child's personal information, and we do not share it for cross-context behavioral advertising (as those terms are defined under the California Consumer Privacy Act). We do not share data with advertisers, and we do not build profiles across other apps.

---

## 5. Children's privacy (COPPA)

**Mukashi Stories is directed to children, and we treat all users as if they were under 13.** This affects everything in this policy:

- **No advertising.** The app contains no ads and is not integrated with any ad network. AdMob is not in the app.
- **No ad personalization.** As described in Section 2, the technical flags that enable ad personalization, ad-related data storage, and ad-user-data sharing are all turned off.
- **No persistent user identity.** We do not collect a name, email, phone number, address, photo, or any other directly-identifying information from the child. We never call `setUserID()`. The Firebase installation ID is a per-install random identifier that resets when the app is reinstalled.
- **Parental controls.** The **Parents** tab is gated behind a 4-digit PIN (and optional biometrics). It gives the parent or guardian full control to:
  - View aggregate stats (stories completed, words saved, reading time)
  - Restrict the visible library to a hand-picked set of stories
  - Set a daily reading time limit
  - Reset reading progress, clear saved words, or reset the onboarding flow
- **Parental contact for COPPA requests.** Parents and guardians can email **mukashi.dev@gmail.com** to request access to, deletion of, or further information about any data associated with their child's device. Because we don't tie data to identifiable children, the most reliable erasure is uninstalling the app — which invalidates the Firebase installation ID and removes all local data.
- **No third-party data brokers.** The only third party that processes data from this app is Firebase (Google), described in Section 6.
- **In-app purchases gated by Apple's parental controls.** All purchases go through Apple's standard In-App Purchase flow, so they're subject to whatever parental controls you've configured on the device — including **Ask to Buy** (Family Sharing) and **Screen Time → Content & Privacy Restrictions → iTunes & App Store Purchases**. We do not have a separate purchase flow that bypasses these controls.

---

## 6. Third parties

The only third-party service the app communicates with is **Firebase**, operated by Google LLC. Google processes Analytics and Crashlytics data as our service provider, under the [Firebase Data Processing and Security Terms](https://firebase.google.com/terms/data-processing-terms). Google's own privacy practices are covered by the [Google Privacy Policy](https://policies.google.com/privacy).

Google primarily processes this data on servers located in the **United States**. For users in the EEA, UK, or Switzerland, international transfers rely on Google's Data Processing and Security Terms, which incorporate the European Commission's Standard Contractual Clauses and the UK International Data Transfer Addendum.

No other third-party analytics, advertising, or tracking SDK is bundled in the app.

---

## 7. How long we keep it

- **Local data** — kept on your device until you delete it or uninstall the app.
- **Firebase Analytics** — Google retains event-level data for **14 months** (Firebase's default), after which older events are aggregated or dropped.
- **Firebase Crashlytics** — Google retains crash reports for **90 days**.

---

## 8. Your rights and choices

- **Reset reading data** at any time — **Parents → Reset Reading Progress** or **Clear Saved Words** (PIN-gated).
- **Turn off analytics system-wide** — iOS **Settings → Privacy & Security → Analytics & Improvements → Share iPhone Analytics**. When this is off, Firebase still receives minimal crash data; you can prevent even that by uninstalling the app.
- **Access or erase your or your child's data** under GDPR (EEA, UK), CCPA/CPRA (California), or similar laws — email **mukashi.dev@gmail.com**. Because we don't tie analytics data to a persistent identity, the most reliable erasure is uninstalling the app, which invalidates the Firebase installation ID.
- **Lodge a complaint** — if you're in the EEA, UK, or Switzerland and believe we're mishandling your data, you have the right to complain to your local data protection authority. We'd appreciate the chance to address your concern first — email **mukashi.dev@gmail.com** and we'll respond within 30 days.

---

## 9. Security

- Local data is stored using iOS's standard app sandbox protections. If you enable App Lock or biometrics for the Parent Dashboard, those areas are additionally gated behind Face ID / Touch ID / passcode.
- Data sent to Firebase travels over HTTPS (TLS).
- We cannot guarantee perfect security — no one can. If we become aware of a breach that affects your data, we will notify you as required by applicable law.

---

## 10. Changes to this policy

If we change this policy, the new version will replace this page at **https://hadicuet.github.io/mukashistories-legal/** and the "Effective date" at the top will be updated. Material changes (e.g. a new third-party service, a new category of data) will be called out in the app's release notes.

---

## 11. Contact us

Questions, requests, or complaints: **mukashi.dev@gmail.com**.
