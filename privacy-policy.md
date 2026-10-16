# Mukashi Stories — Privacy Policy

**Effective date:** October 16, 2026

This policy explains what Mukashi Stories collects, why, and the choices you have. Mukashi Stories is a reading app made for children, so we have written it in plain English. A parent or guardian should be able to read it in a few minutes.

**The short version:** there are no accounts, no ads, and no selling of data. Reading progress and saved words stay on your device. We use Google's Firebase to count how the app is used and to find crashes. Parents decide whether usage counts are shared and whether the app sends story news.

---

## 1. Who we are

Mukashi Stories is an app for reading bilingual children's folk tales. Each line shows the story language and the reader's own language together. It is developed and run by **Abdullah Al Hadi** ("we", "us"). For the EU / UK / EEA General Data Protection Regulation (GDPR) and the California Consumer Privacy Act (CCPA/CPRA), Abdullah Al Hadi is the **data controller** for personal data collected through the app. For any privacy question, write to **mukashi.dev@gmail.com**.

This policy covers the Mukashi Stories app on iPhone, iPad, Mac, and Apple Vision Pro.

---

## 2. What we collect

### Stays on your device

These are stored on your device only. We never receive them.

- **Reading progress** — which page of which story you reached, which stories you finished, and which you marked as loved.
- **Saved words** — words you saved to "My Words", with your review history.
- **Settings** — language pair, theme, text size, layout, narration and reminder choices, and your parental controls.
- **Daily reading minutes** — counted on the device for the parental daily reading limit.
- **Parent PIN** — if a parent sets one, only a scrambled (hashed) version is kept, on the device. We never see the PIN.
- **App Lock** — if turned on, a simple on/off setting on the device.

There are no accounts and no sign-in. If iCloud Backup is on, Apple may include this data in your encrypted backup. That is between you and Apple. A parent can clear it from **Parents → Reset Reading Progress / Clear Saved Words / Reset Onboarding**. Deleting the app removes all of it.

### Usage data (Firebase Analytics, parent can turn off)

We use **Google Firebase Analytics** to learn which features and stories children enjoy. We use the version of Firebase Analytics that has **no advertising features**. The app does not read the advertising identifier (IDFA), does not collect the vendor identifier (IDFV), and does not ask for App Tracking permission.

When usage sharing is on, Analytics receives:

- A random identifier made for this app on this device (the Firebase installation ID). It cannot recognise your child in other apps, and it resets when the app is reinstalled.
- Device type, system version, app version, and language.
- **Approximate location**, such as the country or city, worked out by Google from the connection's IP address. Google does not keep the IP address itself. We do not use GPS and the app has no location permission.
- Screens viewed and taps on features, such as tab switches and setting changes.
- Story activity: which stories are opened, finished, or loved (story ID and title), reading time, and page turns. We never send story text.
- Word activity: that a word was tapped, saved, removed, practised, or pronounced. We send the word itself and its part of speech, to learn which vocabulary children find useful. We never send who tapped it.
- Purchase screen events: that the paywall was shown, a purchase started, finished, or failed, and which plan. We never send prices, receipts, or payment details.
- A few settings (app language pair, theme, layout style) and whether the device has Premium.

We never set a user ID, and we never send names, email addresses, contact details, photos, or anything a child types.

**Your choice:** in **Parents → Share anonymous usage data**, a parent can switch this off at any time. The switch starts **off** in the European Economic Area, the United Kingdom, and Switzerland, and **on** elsewhere. When it is off, the app does not send usage data to Analytics.

### Crash reports (Firebase Crashlytics)

Crash reports help us fix bugs. They are **not** controlled by the usage-data switch. They contain:

- The technical trace of what went wrong.
- The device state at that moment (system version, device model, memory).
- Short log lines such as "opened Reader". They never contain saved words, story text, or personal content.
- Errors the app reports without crashing, such as a failed store lookup.

### Notifications

- **Daily reading reminder** (optional): a reminder that is created and shown on your device at the time you choose. Nothing is sent to us for it.
- **Story news & offers** (optional): if a parent says yes, the device joins Firebase Cloud Messaging topics so we can send news about new stories and offers. The topics are `all_users`, `free` (devices without Premium), and one for the app language (for example `lang_en`), so the message arrives in the right language. We do not keep a list of devices and cannot tell which device is which. Until a parent says yes, the device joins none of these topics and gets no news or offers.
- Notifications need your permission through the iPhone's system prompt. To stop story news, switch off **Settings → Notifications → Story news & offers** in the app, or turn off notifications for the app in iOS Settings.

### Promotional offers (GitHub Pages)

When the app opens, it downloads a small public file (`promo.json`) from our legal pages, hosted on GitHub Pages. The file says whether a special offer is running. The request sends nothing about you or your child, and we add no identifiers. As with any website, **GitHub can see the device's IP address** in the request. See [GitHub's privacy statement](https://docs.github.com/site-policy/privacy-policies/github-general-privacy-statement).

### In-app purchases

Mukashi Stories offers an optional **Premium** subscription and a one-time lifetime unlock through Apple's In-App Purchase system.

- **Apple handles the payment.** The app and we never see your card or payment details.
- **On your device,** the app keeps which product you bought and whether it is active.
- **Restoring purchases** asks Apple which products belong to your Apple ID. We keep no purchase records of our own.

### Contacting support

If you email us from the app, the message may include the app version, system version, device model, language, and theme so we can help you. You can delete these lines before sending. We use your message only to reply.

### What we do not collect

We do not collect names, email addresses, accounts, photos, contacts, precise location, or payment details. The app has no camera, microphone, photo library, contacts, or motion permissions, and it records no audio. Read-aloud uses the voices built into your device and works on the device.

---

## 3. Permissions the app may ask for

- **Face ID / Touch ID / passcode** — optional. Used only if a parent turns on **App Lock** or biometrics for the Parents area. The check is done by Apple on the device. The app never sees your face or fingerprint.
- **Notifications** — optional, as described above.

---

## 4. How we use this data

- **Data on your device** powers the app: picking up where you left off, reviewing saved words, applying your settings. It is used for nothing else.
- **Usage data** tells us which features and stories to improve or drop. We look at totals, not at individual children.
- **Crash reports** tell us when and why the app breaks so we can fix it.
- **Notification topics** let us send news to the right language and audience.

**We show no ads, we do not sell personal information, and we do not share it for advertising.** We do not track your child across other companies' apps and websites.

---

## 5. Children's privacy

Mukashi Stories is made for children, with a parent or guardian in control. We treat every user as a child under 13, and as a child under the age of consent in their country.

- **No ads** and no ad networks. No advertising identifiers are read.
- **No accounts** and no collection of a child's name, email, phone number, address, or photos.
- **Parents decide.** Purchases, outside links, settings, usage sharing and story news sit behind a grown-up check, or behind the parent's 4-digit PIN (optionally Face ID or Touch ID) once one is set. A parent can:
  - Switch usage sharing on or off.
  - Say yes or no to story news and offers.
  - View reading stats, pick which stories are shown, and set a daily reading limit.
  - Reset reading progress, clear saved words, or reset onboarding.
- **Purchases follow your Apple settings.** They go through Apple, so **Ask to Buy** and Screen Time restrictions apply.
- **Only service providers.** The only outside services are Google (Firebase) and GitHub (Pages), described in Section 6, and Apple for purchases and notification delivery.
- **Requests.** Parents can email **mukashi.dev@gmail.com** to ask about, access, or delete data linked to their child's device. Because we hold no accounts or names, the most reliable way to erase it is to delete the app (see Section 8).

We follow the principles of the US Children's Online Privacy Protection Act (COPPA) and Article 8 of the GDPR. If you believe a child has given us personal information, tell us and we will delete it.

---

## 6. Other companies involved

- **Google (Firebase)** processes Analytics, Crashlytics, and Cloud Messaging for us as a service provider, under the [Firebase Data Processing and Security Terms](https://firebase.google.com/terms/data-processing-terms). See also the [Google Privacy Policy](https://policies.google.com/privacy). Google mainly processes this data in the **United States**. For people in the EEA, UK, or Switzerland, transfers rely on the Standard Contractual Clauses and the UK International Data Transfer Addendum in those terms.
- **GitHub** hosts the promo file and this policy (see "Promotional offers").
- **Apple** processes purchases and delivers notifications. Apple's own privacy policy applies.

No other analytics, advertising, or tracking tool is in the app.

---

## 7. How long we keep it

- **On your device** — until you delete it or delete the app.
- **Firebase Analytics** — Google keeps event-level data for 14 months.
- **Firebase Crashlytics** — crash reports are kept for 90 days.
- **Notification topics** — nothing is stored by us about which device joined; topic membership ends when you opt out or delete the app.

---

## 8. Your choices and rights

- **Turn off usage sharing** — **Parents → Share anonymous usage data**.
- **Turn off story news** — **Settings → Notifications → Story news & offers**, or iOS Settings → Notifications.
- **Clear reading data** — **Parents → Reset Reading Progress** or **Clear Saved Words**.
- **Delete everything** — delete the app. This removes all data on the device and gives a reinstalled app a new random identifier, so old usage data can no longer be linked to it.
- **Access or erase data** under GDPR, CCPA/CPRA, or similar laws — email **mukashi.dev@gmail.com**. We hold no names or accounts, so we may ask for details to find the right records, and some data may not be linkable to you.
- **Complain** — if you are in the EEA, UK, or Switzerland, you can complain to your local data protection authority. We would like the chance to help first; we reply within 30 days.

---

## 9. Security

- Data on your device is protected by the standard iOS app sandbox. App Lock and Parents area protection add Face ID, Touch ID, or passcode checks.
- Data sent to Firebase and GitHub travels over HTTPS.
- No system is perfectly secure. If a breach affects your data, we will tell you as the law requires.

---

## 10. Changes to this policy

If we change this policy, the new version will replace this page at **https://hadicuet.github.io/mukashistories-legal/** and the effective date above will change. For material changes, such as a new service or new kind of data, we will say so in the app's release notes.

---

## 11. Contact us

Questions, requests, or complaints: **mukashi.dev@gmail.com**.
