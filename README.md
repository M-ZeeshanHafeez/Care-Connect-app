CARE CONNECT

Project Overview and Store Listing Information
CareConnect is an intelligent, production-grade hybrid medical assistant and medication reminder mobile application developed using Flutter. It features a unique automated system that seamlessly bridges online healthcare data with offline accessibility.

App Details Required for Submission

App Name: CareConnect
Version: v1.0.0 (Release Build)
Category: Medical / Health and Fitness
Target Audience: Caregivers, Patients, and Medical Students.
Developer Coursework: Flutter Mobile App Development (Roll No: 84).

App Description
CareConnect is designed to tackle a critical challenge: ensuring constant access to reliable healthcare information and rigid medication scheduling even in regions with highly unstable internet connectivity.

The application utilizes an advanced Hybrid AI Architecture:

Online Mode (Gemini 1.5 Flash): When internet is available, the app bypasses standard packages to establish a direct, low-latency REST API connection with Google's servers, providing globally comprehensive data on any disease, symptom, or global medicine.

Offline Mode (Fail-Safe Database): Equipped with a built-in 4-second timeout filter, the app intelligently switches to a massive, hardcoded local database containing local top-selling medicines (for example: Panadol, Brufen, Risek, Flagyl, Augmentin, Gravinate) to ensure instantaneous emergency access offline.

Key Features Implemented:

Dynamic Patient Profiles: Create and delete separate profiles for multiple patients.

Smart Medication Alarms: Auto-checks system time to trigger automated alerts for medicine logs.

Stock Management: Decrements medication quantities automatically upon intake and fires 'Low Stock Alerts'.

System Notifications: Fully integrated background notifications using flutter_local_notifications.

Medical Report Vault: Captures, compresses, and securely stores digital camera images of medical reports locally on the device using image_picker with dynamic multi-zoom previews.

Privacy Policy
CareConnect prioritizes user data integrity and strict medical confidentiality.

Zero-Cloud Retention: The app does not transmit personal data, names, or patient profiles to external servers. All information remains on the local device via encrypted SharedPreferences.

Local Image Sandbox: Medical report photos taken via the camera application are stored locally in the application's secure sandbox storage and are not shared with any third-party networks.

AI Data Guardrail: Search queries sent over the secure HTTPS REST endpoint to Google Gemini do not include any identifiable patient credentials.

App Permission Details
To ensure core functionality, the application explicitly requests the following hardware and system level permissions upon installation:

android.permission.CAMERA: Required for the Medical Report Vault to snap live pictures of prescriptions and diagnostic reports.

android.permission.READ_EXTERNAL_STORAGE / WRITE_EXTERNAL_STORAGE: Necessary to save, retrieve, and display local report imagery within the app grid.

android.permission.POST_NOTIFICATIONS: Essential for launching background alerts and time-critical medicine reminders.

android.permission.INTERNET: Utilized exclusively to establish a secure handshake with the Gemini API for infinite medical lookup.
