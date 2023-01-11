---
name: Example Issue
about: Example of the New Issue template
title: 'Implement Forgot Password Feature'
labels: ''
assignees: ''
---

## Description

**Request:** Client ABC would like us to add a "forgot password" button to their login page so that their users can reset their password when forgotten.

**Possible challenges?**

-   Email functionality is likely needed for password reset
-   Simulating different login scenarios when testing
-   A new page will need to be created that users are navigated to when clicking the reset link that is emailed to them

#### Notes:

-   Consider using SendGrid for sending emails

## To Do

-   [ ] Add and style button on login form
-   [ ] Setup API endpoint to handle password reset request
-   [ ] Create Forgot Password modal when button is clicked
    -   [ ] Retrieve and send user info to reset endpoint when button is clicked
-   [ ] Connect API to SendGrid
-   [ ] Send email containing reset link to user's provided email address, if user exists
    -   [ ] Reset link should navigate user to Password Reset page
    -   [ ] Notify user when email has been sent
    -   [ ] Create Password Reset page
        -   [ ] Add password validation to new form field
-   [ ] Create endpoint on User Controller to receive and update new password from user
-   [ ] Notify user of successful/unsuccessful password reset

## Acceptance Criteria / Deliverables

**Required tasks for completion:**

-   [ ] "Forgot password" button allows the user to reset their password
-   [ ] User is notified of successful/unsuccessful password resets, and unsuccessful message provides next steps
-   [ ] Feature is tested, working properly, and is ready to be deployed on **demo server**
-   [ ] Postman tests exist to test all functionality (see ABC/password-reset/)
