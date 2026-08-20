# Development and Debugging with Qoder

## 1. Introduction

After generating and initially testing the application, the next step is to continue development and debugging in Qoder.

Qoder is an AI-assisted development environment that can be used to open the generated project, inspect its code, run the application, and help solve development problems.

The basic workflow is:

Generated Project
↓
Open in Qoder
↓
Run Development Server
↓
Test Application
↓
Find Problem
↓
Ask Qoder to Fix It
↓
Test Again

---

## 2. Open the Project in Qoder

After downloading the generated project from the app-building platform, open that project inside Qoder.

Qoder provides an environment where we can work directly with the project files and use AI assistance while developing the application.

This allows us to move from simply generating the application to actually developing and maintaining it.

---

## 3. Use the Terminal

After opening the project in Qoder, the application's development server can be started through the terminal.

For an Expo application, the development server can be started with:

npx expo start

This starts the Expo development environment and allows the application to be run and tested.

The basic workflow is:

Open Project
↓
Open Terminal
↓
Run Expo Server
↓
npx expo start
↓
Open Application
↓
Test

---

## 4. When the Development Server Produces an Error

Sometimes the project may not start successfully.

For example, the terminal may display an error related to:

- Missing dependencies
- Project configuration
- Package versions
- Expo configuration
- Environment settings
- Other development issues

Instead of trying to guess the solution immediately, the error can be given to Qoder's AI assistant.

For example:

I ran `npx expo start`, but the project is showing this error: [paste the error]. Please diagnose the issue and fix it.

The AI can inspect the project and help determine the cause.

---

## 5. Let the AI Investigate the Project

One advantage of using an AI-assisted development environment is that the AI can work with the project itself.

Instead of only asking a general question such as:

Why is Expo not working?

We can provide the actual terminal error and ask the AI to investigate it.

A useful workflow is:

Run Command
↓
Read Error
↓
Give Error to Qoder
↓
Qoder Inspects Project
↓
Identify Cause
↓
Apply Fix
↓
Run Again

This creates a practical debugging loop.

---

## 6. Test the Application After Starting the Server

Once the Expo server is running, open the application and test it again.

At this stage, check whether the previously generated functionality works correctly.

For example:

- Application launches.
- Navigation works.
- Camera works.
- Images can be selected.
- API requests work.
- AI analysis works.
- Data is saved.
- Dashboard displays the correct information.

The goal is to confirm that the downloaded project is functioning correctly in the local development environment.

---

## 7. Fixing Application Problems with Qoder

If an application feature does not work, the issue can be described directly to Qoder.

For example:

When I click Capture Photo, the camera does not start. Please inspect the relevant code and fix the issue.

Qoder can inspect the project files, identify the relevant code, and suggest or apply changes.

After the change is made, the application should be tested again.

---

## 8. Direct Code Changes

AI assistance is useful, but basic code knowledge is still valuable.

If you understand the relevant code, you can also inspect the file yourself and make a direct change.

For example, if you identify the specific UI component or function responsible for a problem, you can modify the code directly.

This is one of the advantages of working inside a development environment instead of relying entirely on an external app generator.

You can:

- Read the generated code.
- Identify the relevant file.
- Modify the code.
- Save the changes.
- Restart or refresh the application.
- Test the result.

---

## 9. Refreshing the Application

After making a code change, the application needs to reflect the updated code.

During Expo development, the application can be refreshed to load the latest changes.

For example, the terminal or development environment may provide a refresh option.

The important workflow is:

Change Code
↓
Save
↓
Refresh Application
↓
Verify Result

If the change does not produce the expected result, inspect the error and continue debugging.

---

## 10. AI-Assisted vs Manual Debugging

There are two useful approaches.

### AI-Assisted Debugging

Describe the problem to Qoder and allow it to inspect and modify the project.

This is useful when:

- The error is unfamiliar.
- Multiple files may be involved.
- You need help understanding the problem.
- You want to move quickly.

### Manual Debugging

Inspect the code yourself and make the required change.

This is useful when:

- You understand the issue.
- The change is small.
- You want direct control.
- You want to improve your understanding of the codebase.

The strongest workflow is not to choose only one.

Use AI for speed and use your own understanding for verification and control.

---

## 11. Understand Before Accepting a Fix

An AI assistant may be able to modify the code quickly, but that does not mean every generated change is automatically correct.

Before accepting a major change, consider:

- What caused the problem?
- What did the AI change?
- Why should this fix work?
- Could the change affect another feature?
- Does the application still behave correctly?

This helps prevent blindly accepting changes that create new problems elsewhere.

---

## 12. Debugging Workflow

A practical debugging workflow is:

Step 1 — Run the application
↓
Step 2 — Reproduce the problem
↓
Step 3 — Read the error
↓
Step 4 — Identify the affected feature
↓
Step 5 — Give the error and context to Qoder
↓
Step 6 — Let Qoder inspect the project
↓
Step 7 — Review or apply the suggested fix
↓
Step 8 — Run the application again
↓
Step 9 — Test the affected feature
↓
Step 10 — Test related functionality

This approach turns debugging into a repeatable engineering process.

---

## 13. Why Qoder Is Useful in This Workflow

The purpose of using Qoder is not simply to generate more code.

It provides a development environment where we can:

- Work with the generated project.
- Use a terminal.
- Inspect project files.
- Modify source code.
- Run the application.
- Debug problems.
- Use AI assistance during development.

This makes it useful as the next stage after generating an initial application with an AI app-building platform.

---

## 14. Practical Workflow

The complete workflow for this section is:

Step 1 — Download the generated project
↓
Step 2 — Open the project in Qoder
↓
Step 3 — Open the terminal
↓
Step 4 — Run `npx expo start`
↓
Step 5 — Open the application
↓
Step 6 — Test the complete application
↓
Step 7 — Identify errors or missing functionality
↓
Step 8 — Provide the problem and error to Qoder
↓
Step 9 — Let Qoder inspect and fix the project
↓
Step 10 — Review the changes
↓
Step 11 — Refresh or restart the application
↓
Step 12 — Test again
↓
Step 13 — Repeat until the required functionality works correctly

---

## 15. Key Takeaways

- Qoder can be used to continue development after generating an application with an AI app builder.
- The generated project can be opened directly inside Qoder.
- The Expo development server can be started with `npx expo start`.
- Terminal errors can be provided to Qoder for investigation.
- Qoder can inspect project code and help identify problems.
- Developers can also make code changes manually.
- After changing code, the application should be refreshed and tested.
- AI-generated fixes should always be verified.
- Basic programming knowledge remains valuable even when using AI coding tools.
- The best workflow combines AI assistance with developer understanding and verification.

---

## 16. Final Principle

AI can accelerate development, but the developer remains responsible for understanding and validating the result.

Use Qoder to:

**Inspect → Diagnose → Fix → Test → Verify**

Do not treat the AI as a replacement for engineering judgment.

Use the AI for speed, but keep control of the codebase and the final result.