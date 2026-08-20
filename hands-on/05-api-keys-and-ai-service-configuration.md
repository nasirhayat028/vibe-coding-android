# API Keys and AI Service Configuration

## 1. Introduction

After the application is running correctly, the next step is to configure the external AI services that the application depends on.

For the calorie-tracking application, the AI functionality can use services such as:

- Google Gemini
- OpenAI

These services require API credentials so that the application can communicate with them.

The basic workflow is:

Application
↓
AI Service
↓
API Key
↓
API Request
↓
AI Response
↓
Application

---

## 2. Gemini API Key

If the application uses Gemini for AI functionality, a Gemini API key needs to be created.

The key can be obtained through Google AI Studio.

The general process is:

Open Google AI Studio
↓
Sign in
↓
Create or access an API key
↓
Copy the API key
↓
Configure it in the application

The API key allows the application to authenticate requests to the Gemini service.

---

## 3. OpenAI API Key

If the application also uses OpenAI models, an OpenAI API key is required.

The key can be managed through the OpenAI platform.

The general workflow is:

Open OpenAI Platform
↓
Sign in
↓
Create or access an API key
↓
Configure usage or billing limits when required
↓
Add the key to the application

OpenAI usage can generate costs depending on the services and models being used, so usage should be monitored carefully.

---

## 4. Why API Keys Are Required

An API key allows an external service to identify and authorize requests from an application or user.

For example:

Android App
↓
API Request + API Key
↓
Gemini / OpenAI
↓
AI Processing
↓
API Response
↓
Android App

Without valid authentication, the external service may reject the request.

---

## 5. User-Provided API Keys

In the application workflow being developed, users can provide their own API keys.

For example:

User
↓
Open Settings
↓
Enter Gemini API Key
↓
Enter OpenAI API Key
↓
Save Keys
↓
Application Uses Configured Keys

This approach means the application can use the user's own API access instead of requiring the application developer to provide one shared API key for every user.

The application should clearly explain to users how their API keys are handled and stored.

---

## 6. API Usage and Billing

AI APIs may have usage limits or costs.

For example, repeated image analysis or AI requests can increase usage.

Therefore, API usage should be monitored.

For OpenAI, the platform provides usage and billing controls that can be used to monitor consumption and configure limits or alerts where available.

This is important because an application that repeatedly sends requests can unexpectedly increase API usage.

---

## 7. Monitor Usage

When working with external AI services, regularly check:

- API usage
- Number of requests
- Model usage
- Billing
- Usage limits
- Unexpected activity

The goal is to understand how the application is consuming the external service.

This becomes especially important when an application moves from development to real users.

---

## 8. API Configuration in the Application

After obtaining the required keys, configure them according to the application's design.

For example:

Gemini API Key
↓
Application Configuration
↓
Gemini API Request

and:

OpenAI API Key
↓
Application Configuration
↓
OpenAI API Request

The exact configuration method depends on how the generated application has been implemented.

The important principle is that API credentials should be handled securely and should not accidentally be exposed in source code or public repositories.

---

## 9. Test the AI Integration

After configuring the API keys, test the actual AI functionality.

For the calorie-tracking application:

Open Application
↓
Capture Food Image
↓
Send Image for Analysis
↓
AI Service Processes Image
↓
Receive Nutritional Information
↓
Display Result
↓
Save Result

Verify that the complete flow works.

Do not only check whether the API key has been entered.

The actual API request and response should also be tested.

---

## 10. Common API Problems

AI API integrations can fail for several reasons.

Common problems include:

- Invalid API key
- Missing API key
- Incorrect configuration
- API usage limit reached
- Billing or account limitations
- Network problems
- Invalid API request
- Unsupported model
- Incorrect request format
- External service outage

When a problem occurs, inspect the error message and determine whether the issue is related to configuration, authentication, usage, networking, or the application code.

---

## 11. Debugging API Problems

A practical debugging process is:

API Request
↓
Request Fails
↓
Read Error
↓
Check API Key
↓
Check Configuration
↓
Check Model
↓
Check Usage / Limits
↓
Check Request Format
↓
Test Again

If the problem is related to the application code, Qoder can be used to inspect the relevant code and help diagnose the issue.

---

## 12. Security Considerations

API keys are sensitive credentials.

They should not be treated like ordinary text.

Avoid:

- Publishing keys in GitHub repositories.
- Hardcoding secrets into public source code.
- Sharing keys with other people.
- Leaving test keys exposed.
- Sending keys unnecessarily to external services.

If a key is accidentally exposed, it should be revoked or replaced as soon as possible.

The exact security approach depends on whether the key belongs to the developer, backend, or individual user.

---

## 13. API Keys and Local Storage

If users provide their own API keys and the application stores them locally, the storage mechanism should be chosen carefully.

Sensitive credentials should not simply be stored as ordinary unprotected application data.

The application should use an appropriate secure storage mechanism for sensitive information where required.

The goal is:

User API Key
↓
Secure Handling
↓
Application
↓
API Request

rather than:

User API Key
↓
Plain Text File
↓
Application

---

## 14. Practical Configuration Workflow

The complete workflow is:

Step 1 — Identify the required AI services
↓
Step 2 — Create the required API credentials
↓
Step 3 — Configure usage and billing controls
↓
Step 4 — Add the credentials according to the application's design
↓
Step 5 — Test the API connection
↓
Step 6 — Test the actual AI functionality
↓
Step 7 — Monitor API usage
↓
Step 8 — Handle errors and failed requests
↓
Step 9 — Verify that credentials are not exposed
↓
Step 10 — Continue development after successful integration

---

## 15. Key Takeaways

- External AI services require proper authentication.
- Gemini and OpenAI can be integrated through their APIs.
- API keys allow applications to authenticate requests.
- User-provided API keys can be used when the application is designed for that workflow.
- API usage should be monitored carefully.
- Billing and usage limits should be considered.
- API keys are sensitive credentials and must be handled securely.
- Never expose secrets in public repositories.
- Always test the complete API request and response flow.
- API failures should be diagnosed using the actual error information.
- Secure handling becomes increasingly important as the application moves toward production.

---

## 16. Final Principle

API integration is not complete when an API key has simply been added.

A complete integration should be:

**Configured → Authenticated → Tested → Monitored → Secured**

The application should communicate reliably with the external service while protecting credentials and controlling usage.