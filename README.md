# CakeBell Support

If you need help or have questions, please contact:

📧 Email: anaiccial@icloud.com

---

# Privacy Policy for CakeBell

**Last updated: October 19, 2026**

## Overview

CakeBell ("the App") is a birthday reminder application that helps you remember and celebrate your contacts' birthdays. This privacy policy explains how the App handles your data. It also covers this website.

## Controller

Dr. Markus Gäth  
Derkskamp 95  
48163 Münster  
Email: anaiccial@icloud.com

## How to Delete Your Data

CakeBell, developed by Markus Gaeth, lets you delete your server-side data directly in the App — no account or support request needed:

1. Open **CakeBell** on your phone
2. Go to the **Settings** tab
3. Scroll down and tap **"Delete my data"**
4. Confirm by tapping **"Delete"**

This immediately and permanently deletes your synced contact names and birthdays, your reminder settings, and your device's push token from our database (see [What Data We Transmit](#what-data-we-transmit) below for exactly what that covers). Reminders are turned off until you re-enable them, which creates a fresh entry. **There is no additional retention period** — the database record is removed right away, not just deactivated.

If you've already uninstalled the App and still want your data deleted, email **anaiccial@icloud.com** with your approximate last-use date and device type (iOS/Android).

## Data Collection and Storage

### What Data We Access
- **Contact Information**: The App reads contact names and birthdays from your device's address book (full names are only shown inside the App)
- **Contact Photos**: Profile pictures from your contacts (if available) — these are never transmitted
- **User Preferences**: Your settings including reminder times, intervals, and relationship categorizations

### What Data We Transmit
To provide reliable birthday reminders via push notifications, the following data is securely transmitted to our servers:
- **The first name and birthday date** (month and day only) of contacts with birthdays — last names are not transmitted
- **The contact's internal identifier from your address book**, so a birthday you have congratulated can be marked as done
- **Your reminder settings** (reminder time, interval, enabled/disabled, app language and time zone offset)
- **Your device's push notification token** (assigned by Apple/Google, not personally identifiable)

### What Data We Do NOT Transmit
- No last names, phone numbers, email addresses, or photos
- No contact data of people without birthdays
- No message content or communication history
- No device identifiers, location data, or usage analytics

### How We Store Data
- **On your device**: All contact details, relationship types, and message preferences are stored locally using AsyncStorage
- **On our servers**: Only the minimal data listed above is stored in an encrypted AWS DynamoDB database in the EU (Frankfurt, Germany) to schedule push notifications

## Data Usage and Legal Basis

We use the collected data solely to:
- Display upcoming birthdays
- Send push notifications for birthday reminders at your chosen time
- Generate personalized birthday messages (locally on your device)
- Organize contacts by relationship type

Under the GDPR, displaying birthdays and sending reminders is based on Art. 6(1)(b) (providing the App you use). Processing your contacts' first names and birthdays, who do not use the App themselves, is based on Art. 6(1)(f) (legitimate interest in reminding you of their birthdays), limited to first name and day/month of birth.

## Data Sharing

**We do not sell your data, and we do not share it with third parties for advertising or marketing.**

Our processors are Amazon Web Services (database and backend, Frankfurt region, EU) and Expo (650 Industries, Inc., USA) for push delivery. Push notifications are delivered through Expo's push notification service, which acts as a relay to Apple Push Notification Service (APNs) and Google Firebase Cloud Messaging (FCM). The notification text itself includes the first name of the contact whose birthday it is (e.g. "🎂 Anna has a birthday today!"), so that first name passes through Expo, Apple, and/or Google as part of delivering the notification to your device. No other contact data (phone number, email, photo) is included in the notification payload. This involves transfers to the USA. Transfers to Expo are based on the EU Commission's Standard Contractual Clauses (Art. 46(2)(c) GDPR); Apple and Google are certified under the EU-US Data Privacy Framework.

The App interacts with messaging applications (SMS, WhatsApp, Threema, Telegram) only when you explicitly choose to send a birthday message. These interactions are handled directly by the respective apps on your device.

## Permissions

The App requires the following permissions:
- **Contacts**: To read birthday information from your address book
- **Notifications**: To send birthday reminders via push notifications
- **SMS** (optional): To send text messages through your device's messaging app

## Data Retention

- Contact data is refreshed each time you open the App
- Server-side birthday data is overwritten with each sync and only reflects your current contacts
- Daily acknowledgment records (which birthdays you've already congratulated) are automatically reset every day
- User settings remain until you delete the App or request deletion via **Settings → Delete my data**
- Requesting deletion via the App removes your server-side record (names, birthdays, settings, push token) immediately and permanently
- Deleting the App removes all local data. Your server-side record is deleted automatically as soon as a push notification shows that your device is no longer registered, and at the latest 12 months after the App last synced. You can also request deletion by email at any time

## Data Security

- Local data is protected by your device's security measures (passcode, biometric authentication, etc.)
- Server-side data is stored in AWS DynamoDB with encryption at rest in the EU (Frankfurt)
- All communication between the App and our servers uses HTTPS/TLS encryption
- Our backend infrastructure runs on AWS Lambda with no persistent servers, minimizing attack surface

## This Website

This website is hosted on GitHub Pages (GitHub, Inc., 88 Colin P. Kelly Jr. Street, San Francisco, CA 94107, USA). When you visit it, GitHub processes technically necessary data, in particular your IP address, to deliver the page and keep the service secure (Art. 6(1)(f) GDPR). GitHub is certified under the EU-US Data Privacy Framework. See [GitHub's privacy statement](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement). This website uses no cookies, tracking or analytics.

If you contact us by email, we use your details only to answer your request and delete them once it is resolved, unless legal retention obligations apply.

## Your Rights

Under the GDPR you have the right to access (Art. 15), rectification (Art. 16), erasure (Art. 17), restriction of processing (Art. 18), data portability (Art. 20), to object to processing based on Art. 6(1)(f) (Art. 21), and to lodge a complaint with a data protection supervisory authority (Art. 77). Send any request to anaiccial@icloud.com.

You can also:
- Revoke permissions at any time through your device settings
- Turn off **Settings → Enable Reminders** at any time: your server-side record is deleted right away and no data is sent while reminders are disabled. Turning reminders back on starts a fresh sync
- Request deletion of your server-side data (synced names and birthdays, reminder settings, push token) at any time via **Settings → Delete my data** inside the App. This immediately and permanently removes your entry from our database; reminders are turned off until you re-enable them, which starts a fresh sync
- Delete all App data, including local data on your device, by uninstalling the application
- Modify relationship types and messaging preferences within the App

## Children's Privacy

The App does not knowingly collect data from children under 13. The App is designed for general audiences.

## Changes to This Policy

We may update this privacy policy from time to time. Changes will be reflected in the "Last updated" date above.

## Contact

For questions about this privacy policy, please contact:
anaiccial@icloud.com

## Compliance

This App complies with:
- Apple App Store Guidelines
- Google Play Store Guidelines
- General Data Protection Regulation (GDPR) — data is stored in the EU (Frankfurt, Germany)
- California Consumer Privacy Act (CCPA) principles
