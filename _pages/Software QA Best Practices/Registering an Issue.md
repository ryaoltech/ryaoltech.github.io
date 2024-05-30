---
title: "How I register an Issue in Jira"
tags:
    - QA
    - Issue
    - Jira
date: "2024-05-20"
thumbnail: "/assets/img/thumbnail/SoftwareBugs.jpg"
bookmark: true
---

# Best Practices for Registering Issues as a Software QA Engineer
---
This guide outlines the steps to ensure that issues are clearly communicated, well-documented, and actionable.

## 1. Clear and Descriptive Title
---
- Make it Specific: Use a concise and descriptive title that summarizes the issue. Avoid vague terms like "bug" or "issue".

## 2. Detailed Description
---
- **Overview:** Provide a brief overview of the problem.
- **Steps to Reproduce:** List the exact steps needed to reproduce the issue, ensuring anyone can follow them and encounter the same problem.
- **Expected Result:** Describe what should happen if the system is working correctly.
- **Actual Result:** Describe what actually happens.

## 3. Environment Details
---
- **System Information:** Include information about the environment where the issue was found (e.g., operating system, browser, version).
- **Build/Version Number:** Mention the software version or build number where the issue occurred.

## 4. Severity and Priority
---
- **Severity:** Indicate how severe the issue is (e.g., Blocker, Critical, Major, Minor).
- **Priority:** Indicate the priority level (e.g., High, Medium, Low) based on the impact on the project.

## 5. Attachments
---
- **Screenshots and Videos:** Attach any relevant screenshots or videos that show the issue.
- **Logs:** Attach log files if they can help in diagnosing the problem.
- **Additional Files:** Any other relevant files (e.g., data files, configuration files) that can help reproduce or understand the issue.

## 6. Issue Tracking System Usage
---
- **Use Templates:** If your organization has an issue template, use it to ensure consistency.
- **Assign Correctly:** Assign the issue to the appropriate person or team responsible for fixing it.
- **Labels/Tags:** Use relevant labels or tags to categorize the issue (e.g., UI, Backend, Performance).

## 7. Communication and Follow-up
---
- **Comments:** Add any additional comments or updates as the issue progresses.
- **Follow-up:** Ensure the issue is followed up and re-tested once resolved. Update the issue status accordingly.

By following these best practices, you can ensure that issues are registered in a way that is clear, comprehensive, and actionable, facilitating efficient resolution by the development team.

## Example of a mock banking application template I am using
---

>**Title:** [Android][FE] Unable to open deep links - "We're unable to open this link" message is shown
>
>**Description:**
>    [Android][FE] Unable to open deep links - "We're unable to open this link" message is shown
>
>    **Test data:**
>        - Device: Samsung Galaxy S24 Ultra (OS 14) 
>        - Build version: 5.305
>        - Deep Link list:
>            - mobile://banking/transfermoney
>            - mobile://banking/funding
>            - mobile://banking/vault
>    
>    **Steps:**
>        1. Launch Zampona app
>        2. Tap on Deep Link
>        3. Observe
>    
>    **Actual Result:**
>        - Error toast message is shown: "We're unable to open this link".
>
>    **Expected:**
>        - User should be lead to Zampona app with the correspondent screen.
>
>    **Attachment:**
>        - Video01.mp4

