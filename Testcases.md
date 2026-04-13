# Test Cases - Login Feature

Author: Shainaz Sultana
Date: April 2026

---

## TC001 - Login with valid email and password

Requirement: FR-001, FR-006
Priority: High

Precondition:

- User has a registered account
- User is on the login page

Steps:

1. Enter email: test@email.com
2. Enter password: Test@1234
3. Click Login button

Expected Result:

- User logged in successfully
- Redirected to home page
- No error message shown

Actual Result: [fill when testing]
Pass / Fail: [fill when testing]

---

## TC002 - Login with wrong password

Requirement: FR-004
Priority: High

Precondition:

- User is on login page

Steps:

1. Enter email: test@email.com
2. Enter password: wrongpassword
3. Click Login button

Expected Result:

- User NOT logged in
- Error shown: "Invalid email or password"
- User stays on login page

Actual Result: [fill when testing]
Pass / Fail: [fill when testing]

---

## TC003 - Login with invalid email format

Requirement: FR-002
Priority: Medium

Precondition:

- User is on login page

Steps:

1. Enter email: notanemail
2. Enter password: Test@1234
3. Click Login button

Expected Result:

- Error: "Please enter a valid email address"
- User NOT logged in

Actual Result: [fill when testing]
Pass / Fail: [fill when testing]

---

## TC004 - Login with password less than 8 characters

Requirement: FR-003
Priority: High

Precondition:

- User is on login page

Steps:

1. Enter email: test@email.com
2. Enter password: abc
3. Click Login button

Expected Result:

- Error: "Password must be at least 8 characters"
- User NOT logged in

Actual Result: [fill when testing]
Pass / Fail: [fill when testing]

---

## TC005 - Login with empty email field

Requirement: FR-001
Priority: High

Precondition:

- User is on login page

Steps:

1. Leave email field empty
2. Enter password: Test@1234
3. Click Login button

Expected Result:

- Error: "Email is required"
- User NOT logged in

Actual Result: [fill when testing]
Pass / Fail: [fill when testing]

---

## TC006 - Login with empty password field

Requirement: FR-001
Priority: High

Precondition:

- User is on login page

Steps:

1. Enter email: test@email.com
2. Leave password field empty
3. Click Login button

Expected Result:

- Error: "Password is required"
- User NOT logged in

Actual Result: [fill when testing]
Pass / Fail: [fill when testing]

---

## TC007 - Login with both fields empty

Requirement: FR-001
Priority: Medium

Precondition:

- User is on login page

Steps:

1. Leave email field empty
2. Leave password field empty
3. Click Login button

Expected Result:

- Validation errors shown for both fields
- User NOT logged in

Actual Result: [fill when testing]
Pass / Fail: [fill when testing]

---

## TC008 - Account locks after 5 wrong attempts

Requirement: FR-005
Priority: High

Precondition:

- User is on login page
- User has valid account

Steps:

1. Enter wrong password 5 times in a row
2. Try to login a 6th time with correct password

Expected Result:

- After 5th attempt: "Account locked for 30 minutes"
- 6th attempt also blocked even with correct password

Actual Result: [fill when testing]
Pass / Fail: [fill when testing]

---

## TC009 - Login with SQL injection attempt

Requirement: FR-004
Priority: High

Precondition:

- User is on login page

Steps:

1. Enter email: ' OR 1=1 --
2. Enter password: anything
3. Click Login button

Expected Result:

- User NOT logged in
- No database error shown
- System handles safely

Actual Result: [fill when testing]
Pass / Fail: [fill when testing]

---

## TC010 - Successful login redirects correctly

Requirement: FR-006
Priority: High

Precondition:

- User has valid registered account

Steps:

1. Enter email: test@email.com
2. Enter password: Test@1234
3. Click Login button
4. Observe URL and page after login

Expected Result:

- URL changes to home page
- Welcome message shown
- User name visible on page

Actual Result: [fill when testing]
Pass / Fail: [fill when testing]
