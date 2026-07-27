# SprintLab — App Store Submission Package

**App version:** 1.0.0 · **Platform:** iOS (iPhone) · **Price:** Paid (one-off) · **Rating:** 4+ · **Bundle ID:** `com.sdtuk.sprintlab`
All copy respects App Store Connect field limits (name ≤30, subtitle ≤30, promo ≤170, description ≤4000, keywords ≤100).

---

## App name & subtitle

- **Name:** `SprintLab` (9)
- **Subtitle:** `Sprint readiness & analytics` (28)

## Promotional text (≤170, editable without review)

> Your daily readiness score, PBs, and the training insights that actually move the needle — all on your phone. No account, no cloud. Built for sprinters. (150)

## App description (≤4000)

```
SprintLab is a pocket performance lab for sprinters — track & field athletes,
masters sprinters, and the coaches who train them. Log your bests, track
training, and let SprintLab turn your data into a daily readiness call and
real performance insights. Everything lives on your device.

PERFORMANCE READINESS
• A 0-100 readiness score each day, with a clear call: Sprint, Gym, Recovery
  or Rest
• Blends sleep, recovery, HRV, resting heart rate, body temperature and
  stress with your own energy, motivation and leg-freshness check-in
• Every value is editable by hand and labelled by source (Manual, Oura,
  Calculated, Estimated)
• Insights like "Today matches your previous personal-best days" and "HRV is
  12% above your monthly average"

PERFORMANCE ANALYTICS
• Automatically finds the relationships that matter: sleep vs 100m time, HRV
  vs top speed, stress vs performance, gym load vs speed and more
• Correlations, trends, and the recovery conditions your personal bests
  actually happen in
• Gets sharper the more you log — the analysis grows with your data

WEARABLE SYNC (OPTIONAL)
• Connect an Oura Ring to auto-fill sleep, recovery, HRV, resting heart rate,
  temperature and stress
• Sign-in uses the vendor's official, secure flow — SprintLab never sees your
  password
• Health data is stored on your device; disconnect any time
• Not required — the whole app works with manual entry alone

PERSONAL BEST TRACKER
• PBs by distance from 30m to 400m and custom distances
• Electronic and hand timing kept separate; a hand time never overwrites an
  electronic record
• Wind readings with automatic wind-legality flags (over +2.0 m/s is marked
  wind-aided, never a legal PB)
• Block, standing and flying starts tracked separately
• PB celebrations that tell you exactly which time you beat

TRAINING DASHBOARD
• Log sessions in seconds: type, timed reps, gym work, notes, injuries, sleep
• Progress graphs per distance and improving/declining trends
• A training consistency score that rewards showing up, week after week

TOOLS
• Sprint calculator: speeds (m/s, km/h, mph), equal-speed equivalents and
  even-pace splits
• WMA-style age grading for masters athletes, fully offline

PRIVATE BY DESIGN
• Your data is stored on your device
• No account, ever
• Full backup export and import you control
• Delete everything in two taps

Built with dark mode, VoiceOver and Dynamic Type throughout.

Whether you're chasing a school record, a masters title, or your first
sub-13 100m, SprintLab keeps the numbers straight so you can focus on
running fast.
```
(~2,150 chars.)

## Keywords (≤100, comma-separated, no app name, no brand names)

```
sprint,track,athletics,100m,200m,masters,pb,readiness,recovery,hrv,wearable,analytics,speed
```
(91) — deliberately excludes brand names (e.g. "Oura") to avoid metadata rejection.

## Support & marketing URLs

- **Support URL** (required): a simple page under your domain, e.g. `https://sdtuk.com/sprintlab` (or a contact page). Support email: `support@sdtuk.com`.
- **Marketing URL** (optional): your product page if you make one.

---

## Pricing — paid, one-off

This is a **paid app** (pay once to download); no in-app purchases, no subscription.

1. **Agreements, Tax, and Banking → Paid Applications** agreement must show **Active**, with bank + tax details completed. *You cannot sell until this is done — do this first.*
2. In the app's **Pricing and Availability**, choose a price point (e.g. **£4.99 / USD 4.99**, adjust to taste) and the countries to sell in.
3. No StoreKit code is needed — Apple charges at download.

> If you later want free download + a one-time in-app unlock instead, that needs an added non-consumable in-app purchase (StoreKit code) — not included here.

---

## Privacy information

**App Store Connect privacy label:** **Data Not Collected.** SprintLab has no accounts, no analytics/advertising SDKs, and stores everything on-device. Health data synced from a wearable stays on the device.

**On the optional wearable relay:** connecting Oura uses a small sign-in relay (Cloudflare) that brokers the OAuth token exchange so the confidential app secret never ships in the binary. It transmits only the sign-in exchange, retains nothing, and never receives your health data (that comes straight to your phone). This is transient, functional data handling — it does not constitute developer data collection — so "Data Not Collected" remains accurate. It is disclosed in the Privacy Policy.

**Privacy questionnaire answers:**
| Question | Answer |
|---|---|
| Does the app collect data? | No |
| Third-party analytics / advertising? | No |
| Tracking (ATT / IDFA)? | No |
| Account required? | No accounts exist |
| Health data used? | Optional, on-device only; never collected by the developer |
| Data leaves the device? | Only when the user exports a backup via the iOS share sheet, to a destination they choose |

**Privacy policy URL** (required): host `PRIVACY_POLICY.md` publicly and paste the URL. **Terms of Service** (`TERMS_OF_SERVICE.md`) can be linked from the same site.

**In-binary declarations already shipped:** iOS privacy manifest (UserDefaults CA92.1, file timestamp C617.1, boot time 35F9.1, disk space E174.1) and `usesNonExemptEncryption=false`.

## Age rating

All content descriptors **None**; unrestricted web access **No** (the only web use is the optional wearable sign-in page); gambling **No**; user-generated content shared with others **No**. Expected rating: **4+**.

---

## Release notes — v1.0.0

```
Welcome to SprintLab — your training data, on your phone, nobody else's.

• Performance Readiness: a daily 0-100 score and a Sprint / Gym / Recovery /
  Rest call from your recovery signals and check-in
• Performance Analytics: automatic correlations and personal-best conditions
  that sharpen as you log
• Optional Oura sync to auto-fill recovery metrics (works fully manual too)
• Personal best tracker with wind-legality and separate electronic/hand times
• Training log, progress trends, and a consistency score
• Sprint calculator and offline age grading for masters athletes
• Dark mode, VoiceOver and Dynamic Type

No account. No ads. No cloud. Fast like you.
```

## Screenshot plan (6.7" @ 1290×2796 required; reuse for 6.1")

Capture in dark mode with seeded data (log ~8 sessions, 5 PBs, and enter a week of daily metrics first). The first two do the selling:

| # | Screen | Caption |
|---|---|---|
| 1 | Ready tab: big readiness score + Sprint recommendation + insights | "Know exactly how to train today" |
| 2 | Analytics: a correlation + PB-condition insight | "The insights that actually move the needle" |
| 3 | PB tracker with gold badges, wind & FAT/HT chips | "PBs tracked like the sport really works" |
| 4 | Training dashboard: consistency score, weekly bars, progress chart | "Your whole season, one screen" |
| 5 | Ready tab metric grid with source badges (Oura / Manual) | "Every number, from your ring or by hand" |
| 6 | Settings data card / Home light mode | "No account. No cloud. Your data stays here" |

---

## Reviewer notes (App Store Connect "Notes")

> SprintLab is fully local: no account, no login, no server required to use
> it. To exercise features: (1) open the Ready tab and tap any metric to
> enter a value — the readiness score and recommendation update; (2) add a
> personal best from the + on the PBs tab; (3) log a session on the Train
> tab; (4) open Performance Analytics from the Ready tab (insights appear
> once enough data is logged); (5) Sprint Calculator and Age Grading are
> under Tools.
>
> The Oura wearable connection is OPTIONAL and requires a physical Oura Ring
> and account, so it cannot be tested in review — the entire app works with
> manual entry and needs no device or login. Age grading uses approximate
> offline tables (labelled in-app). Backup export/import uses the standard
> iOS share sheet / document picker; no data leaves the device otherwise.

---

## Submission checklist

**Done in this repository:**
- [x] Bundle ID `com.sdtuk.sprintlab`, version 1.0.0, portrait iPhone, 4+ posture
- [x] App icon (1024px), dark splash, adaptive icon
- [x] iOS privacy manifest & `usesNonExemptEncryption=false`
- [x] 233 automated tests green; typecheck clean; offline-invariant enforced
- [x] EAS build/submit profiles (`eas.json`), static config (no eas init hang)
- [x] Listing copy, keywords, release notes, screenshot plan, privacy/terms text (this package)

**Remaining — accounts/hardware outside the repo:**
1. App Store Connect: **complete the Paid Applications agreement + banking/tax** (blocks selling).
2. Create the app record with bundle ID `com.sdtuk.sprintlab`; set it to a paid price tier.
3. `eas init` → `eas build --platform ios --profile production` → `eas submit --platform ios`.
4. Host `PRIVACY_POLICY.md` (and `TERMS_OF_SERVICE.md`) at public URLs; paste the privacy URL.
5. Capture the 6 screenshots per the plan on a 6.7" simulator/device.
6. Enter metadata + privacy label ("Data Not Collected") + age rating + reviewer notes, attach the build, submit.
