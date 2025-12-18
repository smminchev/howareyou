# Google Play Data Safety Form Answers

**App:** How Are You?!
**Privacy Policy URL:** `https://[username].github.io/whereareyou/privacy-policy.html`
**Last Updated:** 2025-12-18

## Data Safety Form Responses

### Data Collection and Security

#### Location Data
- **Collected:** YES
- **Shared with third parties:** YES (family members during emergencies only)
- **Purpose:** Emergency detection
- **Data type:** Precise location (GPS coordinates)
- **How it's used:**
  - Emergency detection when app is closed or not in use
  - Safe zone identification
  - Location deviation alerts
- **Privacy reassurance:** "Your location is NEVER shared except during emergencies. All data stays on your device."

#### Personal Information (Email Addresses)
- **Collected:** YES
- **Shared with third parties:** NO
- **Purpose:** App functionality (alert recipients configured by family)
- **Data type:** Email addresses
- **How it's used:** Alert recipient configuration only

#### Sensor Data (Motion Sensors)
- **Collected:** YES
- **Shared with third parties:** NO
- **Purpose:** Pattern learning and emergency detection
- **Data types:**
  - Accelerometer data
  - Gyroscope data
  - Barometer data
- **How it's used:**
  - Detect activity levels and unusual stillness
  - Learn daily routines
  - Emergency detection

#### Device Identifiers
- **Collected:** YES
- **Shared with third parties:** NO
- **Purpose:** App functionality
- **Data type:** Android ID
- **How it's used:** Internal app functionality only

### Security Practices

#### Encryption in Transit
- **Status:** YES
- **Method:** TLS 1.3
- **Details:** Emergency alerts sent via Gmail API are encrypted during transmission

#### Encryption at Rest
- **Status:** YES
- **Method:** SQLCipher
- **Details:** All behavioral data stored locally using Room database with SQLCipher encryption

#### Data Deletion
- **Users can request deletion:** YES
- **Methods:**
  1. "Reset Learning" button - immediate deletion of all behavioral data
  2. App uninstall - automatic deletion by Android
- **Details:** Complete control over data lifecycle, no cloud backups

### Background Location Declaration

**Required explanation for background location usage:**

> This app uses background location for critical safety features:
>
> - **Emergency detection when app is closed or not in use** - Continuous monitoring even when phone screen is off
> - **Safe zone identification** - Learning your regular locations (home, park, coffee shop)
> - **Location deviation alerts** - Detecting when you've moved outside normal patterns
>
> **Privacy reassurance:** Your location is NEVER shared except during emergencies. All data stays on your device.

### Data Handling Summary

**What data is collected:**
- Precise GPS coordinates (location data)
- Motion sensor data (accelerometer, gyroscope, barometer)
- Activity patterns (sleep schedules, stillness duration, daily routines)
- Email addresses (alert recipients)
- Device identifiers (Android ID)
- Safe zone patterns (learned locations)

**How data is used:**
- Emergency detection (unusual stillness, abnormal sleep, location deviations)
- Behavioral pattern learning (30-day learning phase)
- Emergency alerts to family (GPS coordinates + timestamp only)
- Monthly pattern recalibration

**How data is NOT used:**
- NO advertising or marketing
- NO analytics or user tracking
- NO third-party sharing (except emergency alerts to configured family emails)
- NO data selling or secondary use

**Security measures:**
- 100% local storage on device (Room database with SQLCipher)
- ZERO cloud transmission of behavioral data
- OAuth tokens in Android Keystore
- TLS 1.3 encryption for emergency alerts
- On-device AI processing (Gemini Nano)

**Data retention:**
- Retained until app uninstall OR "Reset Learning" triggered
- Immediate deletion on uninstall (Android auto-delete)
- Immediate deletion on "Reset Learning" button
- No cloud backups

## Privacy Policy Sections

All three language versions (English, Bulgarian, German) include:

### 9 Required Sections:
1. Information We Collect
2. How We Use Information
3. Data Storage and Security
4. Data Sharing
5. Data Retention and Deletion
6. Your Rights
7. Children's Privacy
8. Changes to Privacy Policy
9. Contact Information

### 8-Point Legal Framework:
1. Not a Medical Device disclaimer
2. Emergency Services Disclaimer (does not replace 911/112)
3. No Guarantees (false negatives/positives possible)
4. User Responsibility (correct configuration, testing)
5. Privacy Policy Statement (on-device only, no cloud)
6. Limitation of Liability (missed emergencies, technical failures)
7. Informed Consent (parent must know, no secret monitoring)
8. Terms Acceptance (by using app, users accept terms)

## Accessibility Compliance

- **WCAG 2.1 AA+ compliance:** Exceeds standard
- **Contrast ratio:** 6:1 (exceeds 4.5:1 minimum)
- **Font size:** 18px (exceeds 16px minimum, elderly-friendly)
- **Mobile-responsive:** Works on 375px to 1024px+ screen widths
- **Semantic HTML5:** Screen reader compatible
- **Load time:** < 2 seconds (static HTML, minimal CSS, no JavaScript)

## URLs

- **English (PRIMARY):** `https://[username].github.io/whereareyou/privacy-policy.html`
- **Bulgarian:** `https://[username].github.io/whereareyou/privacy-policy-bg.html`
- **German:** `https://[username].github.io/whereareyou/privacy-policy-de.html`

---

## Notes for Play Console Submission

1. **Privacy Policy URL:** Use the English version as the primary URL in Data Safety form
2. **Background Location:** The privacy policy includes the required explanation for background location usage
3. **Data Safety Form:** All answers are derived directly from the privacy policy content
4. **Transparency:** The privacy policy emphasizes local storage, no cloud surveillance, and emergency-only sharing
5. **Legal Protection:** 8-point legal framework provides comprehensive liability disclaimers

---

**Developer Contact:** stoyan.shopov@gmail.com
**Last Updated:** 2025-12-18
