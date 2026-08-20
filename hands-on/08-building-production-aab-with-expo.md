# Building a Production AAB with Expo

## 1. Introduction

After developing, testing, and debugging the Android application, the next major step is preparing it for the Google Play Store.

Android applications submitted to Google Play need to be packaged into an appropriate release format.

For this workflow, Expo is used to create a production Android App Bundle (AAB).

The overall workflow is:

Development
↓
Testing
↓
Debugging
↓
Production Build
↓
AAB File
↓
Google Play Console
↓
Play Store

---

## 2. Why a Production Build Is Required

The development version of an application is mainly used for testing.

Before publishing the application, we need to create a production build.

A production build is prepared for distribution and can be uploaded to Google Play.

For this workflow, the required output is an `.aab` file.

AAB stands for:

**Android App Bundle**

The AAB contains the application package that Google Play can use to deliver the application to Android devices.

---

## 3. Expo as the Build Platform

Expo provides cloud-based services that can be used to build Android applications.

The general workflow is:

Expo Account
↓
Project
↓
Production Build
↓
AAB File

This means the application build can be created using Expo's cloud infrastructure instead of manually configuring the complete Android build environment locally.

---

## 4. Create an Expo Account

To use Expo's cloud build services, create an account on Expo.

The basic workflow is:

Open Expo
↓
Create Account
↓
Sign In
↓
Connect Project
↓
Prepare Production Build

Once the account is ready, the project can be used with Expo's build services.

---

## 5. Building the AAB from Qoder

After opening the project in Qoder, the application can be prepared for a production build.

The AI assistant in Qoder can be instructed to create a production AAB build.

For example:

Create an AAB build for production.

Qoder can then guide the project through the required Expo build process.

The first time the build process is used, authentication may be required.

---

## 6. First-Time Authentication

When using Expo's build services for the first time, the project may ask you to log in to your Expo account.

The basic workflow is:

Start Production Build
↓
Expo Login Required
↓
Sign In
↓
Authenticate Project
↓
Continue Build

After authentication is completed, the production build process can continue.

---

## 7. Build the Production AAB

Once authentication and configuration are complete, the production build can start.

The workflow is:

Project
↓
Production Build Command
↓
Expo Cloud Build
↓
Build Process
↓
AAB Generated

The build process may take some time because the application is being prepared for production distribution.

---

## 8. Download the AAB File

After the build completes successfully, an Android App Bundle is generated.

The `.aab` file can then be downloaded.

The workflow is:

Build Complete
↓
AAB Generated
↓
Download AAB
↓
Prepare for Play Store

This AAB file is the file that will later be uploaded to Google Play Console.

---

## 9. Expo Build Limits

The course workflow notes that Expo provides a limited number of cloud builds depending on the account or plan.

For the workflow being practiced, the available monthly build allowance is sufficient for the expected development and publishing process.

Because cloud builds are a limited resource, production builds should be created intentionally rather than repeatedly rebuilding without a reason.

---

## 10. Verify the Production Build

Before submitting the application to the Play Store, the production build should be treated as an important release artifact.

Make sure:

- The build completed successfully.
- The AAB file was generated.
- The application functionality has already been tested.
- Required API configuration is available.
- Important features work correctly.
- The application is ready for release testing.

Do not consider the application production-ready simply because an AAB file was successfully generated.

A successful build only confirms that the application was packaged successfully.

---

## 11. Development Build vs Production Build

It is important to understand the difference.

### Development Stage

The application is being:

- Built.
- Tested.
- Debugged.
- Modified.
- Refined.

### Production Stage

The application is being:

- Packaged.
- Release tested.
- Submitted.
- Distributed.

The workflow therefore becomes:

Development
↓
Testing
↓
Debugging
↓
Release Preparation
↓
Production AAB
↓
Play Store Testing
↓
Production Release

---

## 12. Production Build Workflow

The complete hands-on workflow is:

Step 1 — Finish the major application functionality
↓
Step 2 — Test the application
↓
Step 3 — Fix important issues
↓
Step 4 — Create an Expo account
↓
Step 5 — Open the project in Qoder
↓
Step 6 — Start the production build process
↓
Step 7 — Authenticate with Expo when required
↓
Step 8 — Wait for the cloud build to complete
↓
Step 9 — Download the generated AAB file
↓
Step 10 — Keep the AAB ready for Play Store testing

---

## 13. Key Takeaways

- A production build is required before distributing the application through Google Play.
- Android applications can be packaged as an Android App Bundle (`.aab`).
- Expo can provide cloud-based Android build services.
- An Expo account is required for this workflow.
- Qoder can be used to initiate and manage the production build process.
- The first build may require Expo authentication.
- After a successful build, the AAB file can be downloaded.
- Cloud build resources should be used carefully.
- A successful AAB build does not automatically mean the application is ready for production.
- The production artifact should be tested before final release.

---

## 14. Final Principle

**Build → Verify → Package → Test → Release**

Creating the AAB is an important milestone, but it is not the final step.

The AAB is the release artifact that moves the application from development into the Play Store publishing workflow.