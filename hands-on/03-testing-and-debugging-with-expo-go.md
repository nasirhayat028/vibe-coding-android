# Testing and Debugging with Expo Go

## 1. Introduction

After generating the application with Bolt, the next step is to test the application on a real device.

For this hands-on workflow, Expo Go is used to preview and test the generated application.

The purpose of this stage is to verify that the application actually works as expected before moving to further development.

The basic workflow is:

Bolt
↓
Generated Application
↓
Expo Go
↓
Run Application
↓
Test Features
↓
Identify Problems
↓
Fix Problems
↓
Test Again

---

## 2. What Is Expo Go?

Expo Go is an application that allows developers to run and preview Expo-based applications on a mobile device during development.

Instead of immediately creating a production build, we can use Expo Go to quickly see how the application behaves on a real Android device.

This is especially useful during the early development and testing stage.

---

## 3. Why Use Expo Go?

When an AI tool generates an application, we need to verify the result.

A browser preview alone may not reveal problems related to actual mobile-device functionality.

For example, an application may contain features such as:

- Camera access
- Gallery access
- File access
- Device permissions
- Touch interactions
- Mobile navigation

Testing on an actual Android device gives us a better understanding of how these features behave in a real environment.

---

## 4. Install Expo Go

To test the application on an Android device, install the Expo Go application on the device.

Once Expo Go is available, it can be used to open the development version of the application.

The development environment and the Android device need to be able to communicate with each other so that the application can be loaded and tested.

---

## 5. Run the Application

After the project has been generated, start the Expo development server from the project environment.

The application can then be opened through Expo Go.

The basic workflow is:

Project
↓
Start Development Server
↓
Expo Development Server
↓
Connect Android Device
↓
Open Application in Expo Go
↓
Test Application

The exact connection method can depend on the development environment and network configuration.

---

## 6. Test the Complete Application Flow

Do not only check whether the application opens.

Test the complete user journey.

For example, for a calorie-tracking application:

Open App
↓
Navigate to Main Screen
↓
Select Food Capture
↓
Open Camera
↓
Capture Image
↓
Send Image for Analysis
↓
Receive Result
↓
Display Nutritional Information
↓
Save Information
↓
Open Dashboard
↓
Verify Daily Tracking

Testing the complete flow helps reveal problems that may not be visible when checking individual screens.

---

## 7. Check Important Features

During testing, verify the application's main functionality.

Check:

- Navigation
- Buttons
- Forms
- Camera
- Gallery
- File access
- API requests
- AI responses
- Local data storage
- Dashboard information
- Error handling
- Permission requests

Every important feature should be tested according to the original application requirements.

---

## 8. Testing Device-Specific Features

Some functionality cannot be properly validated without a real device.

For example, suppose the application contains a camera feature.

You may discover:

The application opens successfully, but clicking Capture Photo does not start the camera.

This is a real application problem even though the rest of the interface may look correct.

Testing on the actual device helps identify these kinds of issues.

---

## 9. Example: Camera Problem

Suppose the user clicks:

Capture Photo

but nothing happens.

The expected behavior is:

Capture Photo
↓
Camera Opens
↓
User Captures Image
↓
Image Preview Appears

If this does not happen, the issue should be reported clearly to the AI development tool.

For example:

When I click Capture Photo, the camera is not starting. Fix the camera functionality so that the camera opens correctly and allows the user to capture an image.

After the fix is applied, test the feature again.

---

## 10. The Test → Fix → Test Cycle

AI-assisted development is usually iterative.

The process is:

Test
↓
Find Problem
↓
Explain Problem
↓
Apply Fix
↓
Test Again

This cycle can happen multiple times.

The important thing is to verify that the fix actually solved the problem instead of assuming that the AI's response means the issue is resolved.

---

## 11. Report Problems Clearly

When reporting a problem to an AI development tool, describe three things:

### 1. What You Did

Example:

I clicked the Capture Photo button.

### 2. What Happened

Example:

The camera did not start.

### 3. What Should Happen

Example:

The camera should open so the user can capture a photo.

This creates a clear problem statement.

A good debugging request follows this pattern:

Action → Actual Result → Expected Result

---

## 12. Do Not Assume the Application Works

An application can look visually complete while still containing functional problems.

For example:

- A button may not perform its action.
- A camera may not open.
- An API request may fail.
- Data may not be saved.
- Navigation may lead to the wrong screen.
- Permissions may not be handled correctly.

Therefore:

**Visual completion ≠ Functional completion**

The application should be tested based on behavior, not appearance alone.

---

## 13. Test After Every Important Fix

After an issue is fixed, test the affected functionality again.

If possible, also test related functionality because one change can sometimes affect another part of the application.

For example:

Camera Fix
↓
Test Camera
↓
Capture Image
↓
Preview Image
↓
AI Analysis
↓
Save Result
↓
Dashboard

This verifies the complete chain rather than only checking whether the camera opens.

---

## 14. Practical Testing Workflow

The complete workflow is:

Step 1 — Install Expo Go
↓
Step 2 — Start the Expo development server
↓
Step 3 — Connect the Android device
↓
Step 4 — Open the application in Expo Go
↓
Step 5 — Test the main application flow
↓
Step 6 — Test important features individually
↓
Step 7 — Check device permissions
↓
Step 8 — Identify errors or missing functionality
↓
Step 9 — Describe problems clearly to the AI tool
↓
Step 10 — Apply the fix
↓
Step 11 — Test the affected feature again
↓
Step 12 — Test the complete flow again

---

## 15. Key Takeaways

- Expo Go can be used to preview and test an Expo application on an Android device.
- Testing should happen after the application is generated.
- A real device can reveal problems that may not appear in a simple preview.
- Test the complete user journey, not just individual screens.
- Camera, gallery, permissions, API calls, storage, and navigation should all be tested.
- AI-generated applications can contain functional problems even when the UI looks correct.
- Clearly explain what you did, what happened, and what should have happened.
- Always verify that an AI-generated fix actually works.
- Use the Test → Fix → Test cycle throughout development.
- Functional correctness is more important than simply having a visually complete application.

---

## 16. Final Principle

**Do not trust the generated application until you have tested it.**

Generate quickly.

Test realistically.

Find problems.

Fix them.

Test again.

A working application is not defined by how good the generated code looks. It is defined by whether the user can successfully complete the intended workflow.