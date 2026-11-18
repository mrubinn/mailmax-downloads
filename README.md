# MAILMAX beta

A keyboard-first desktop email app for Gmail and Google Workspace, with multiple accounts, rich messages, attachments, and inline replies.

**[Download the beta](https://github.com/mrubinn/mailmax-downloads/releases/tag/beta)**

The release page lists the installers currently available for Windows, Apple Silicon Macs, and Intel Macs. Only use a platform file when it is listed there. No developer tools or Google client secrets are needed: install MAILMAX and choose **Sign in with Google**.

## Before signing in

The beta organizer must add your Google account to the approved tester list. Google may show an unverified-app warning, and Gmail access expires after seven days while the app is in Testing. Reconnect through the app when asked. Work or school accounts may need their administrator's approval.

## Installation

- **Windows:** download the .exe and run the installer. The trial installer is unsigned, so Windows may show an unknown-publisher warning.
- **Mac:** download the file matching your processor, open the .dmg, and drag MAILMAX into Applications. The free beta is not Apple-notarized. If macOS cannot verify its developer, use Apple's per-app Open Anyway option in System Settings > Privacy & Security after checking the download source. Do not disable Gatekeeper globally. See [Apple's instructions](https://support.apple.com/en-us/102445).

## Updates and data

Startup checks and automatic downloading default on; change them in Settings > Updates. Windows installs a verified update when you close MAILMAX after saving drafts. Pending sends postpone installation. Mac beta updates are downloaded for you to open and replace the application manually.

Your app connects directly to Google. Mail is cached locally and account tokens are protected using operating-system encryption. This download repository does not receive your mailbox or saved sign-ins. Cloud scheduling and AI features are unavailable during this beta.

## Read receipt privacy

Starting with MAILMAX 0.12.0, outgoing read receipts are the default choice after you review the first-send disclosure. You can send without tracking or change the setting for each account under Settings → Reading. Sharing your verified MAILMAX opens is a separate opt-in.

The receipt service runs on Google Cloud. It receives a Google sign-in token to verify your identity and the recipient addresses needed to match verified opens. It keeps hashed account and recipient lookup values, opening timestamps, and the email addresses of MAILMAX readers who opt in to sharing a verified open. Only the sender can retrieve that message’s receipt history. The service does not receive your Gmail access token, refresh token, message body, subject, or attachments.

An external email app may load a small image and register an External open. Image blocking, caching, and preloading can affect those events. The service retains receipt records for up to 90 days. Disabling outgoing tracking affects future messages. Tracking images already sent remain active until their records expire.

Contact your beta organizer privately with questions about receipt data.

## Feedback

Send feedback privately to the person who invited you. Include your app version, operating system, and reproduction steps. Avoid posting message bodies, attachments, passwords, or tokens in public issues. Keep another way to access Gmail available while testing.
