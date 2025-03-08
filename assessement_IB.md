**Questions to Clarify:**
1. What should happen if someone tries to sign up with an email that’s already taken? Should they get an error message?
2. Does the temporary password need to meet any security requirements (like special characters or numbers)?
3. If a name is too short or too long, should an error message appear? What should it say?
4. Can people use special characters or spaces in their first or last name?
5. What’s the process if the user doesn’t receive the email with their temporary password?



**Test Scenarios:**

1. **Creating a User Successfully**
   - **Steps:**
     1. Enter a valid email, first name (between 6-10 characters), and last name (between 6-12 characters).
     2. Click the "Save" button.
     3. Check if a success message appears and if an email with a temporary password is sent.
   - **Expected Result:** The user is created successfully and receives their login details via email.

2. **Name Length Issues**
   - **Steps:**
     1. Try entering a first or last name that’s too short (less than 6 characters) or too long (over the limit).
     2. Click "Save".
   - **Expected Result:** The system should show an error message and not allow the user to be created.

3. **Checking for Duplicate Emails**
   - **Steps:**
     1. Try to sign up with an email that’s already in use.
     2. Click "Save".
   - **Expected Result:** The system should show an error message saying that the email is already registered.

4. **Verifying Data is Stored Correctly**
   - **Steps:**
     1. Create a new user.
     2. Check the database (`tblUser`) to see if the email, first name, and last name are saved correctly.
   - **Expected Result:** The user’s details should be stored in the right fields with the correct formatting.

5. **Logging In and Checking the Homepage**
   - **Steps:**
     1. Log in with the new user’s credentials.
     2. Check if their name and email are displayed correctly on the homepage.
   - **Expected Result:** The homepage should display a welcome message with the user’s name, just like in the specifications.

