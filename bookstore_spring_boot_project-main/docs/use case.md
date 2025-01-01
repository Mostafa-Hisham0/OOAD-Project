
### **signup**
- **Description**:
    - user creates new acount by ading his bersonal information .
- **Actors**:
    - User
    - staff
- **Preconditions**:
    - The user is not registered in the system.
- **Steps**:
    - Step 1 : user open the system.
    - step 2 : The user clicks the "sign in" button.
    - step 3 : user enter his information(required information)
    - step 4 : The user clicks the "Submit " button.
    - step 5 ; chick if this information are true by verifying his mail 
    - step 6 : open mail and chick the coming maill from the system 
    - step 7 : click the verify mail 
- **Alternative Scenario**:
    - Alternative 1 week password :
      - user try to rewrite new password that stronger than first one
      - The user clicks the "sign in" button.

   - Alternative 2 mail does not exist :
      -user chick if he/she write the mail right
      - The user clicks the "sign in" button.
   
  - Alternative 3 : this mail already exist :
     - user go to login page and try to add the mail 

---

### **Login Use Case**

- **Description**:
    - A registered user logs into the system by providing their credentials.

- **Actors**:
    - User

- **Preconditions**:
    - The user is already registered in the system.

- **Steps**:
    - *Step 1*: The user opens the system.
    - *Step 2*: The user clicks the "Login" button.
    - *Step 3*: The user enters their credentials (username and password).
    - *Step 4*: The user clicks the "Submit" button.
    - *Step 5*: The system checks if the credentials are correct.
    - *Step 6*: If valid, the user is redirected to the system.

- **Alternative Scenarios**:
    - *Alternative 1: Incorrect Password*:
        - The system displays an error message.
        - The user tries to re-enter the correct password and clicks "Submit."

    - *Alternative 2: User Forgot Password*:
        - The user clicks the "Forgot Password" link.
        - The system prompts the user to enter their registered email.
        - The system sends a password reset email.
        - The user clicks the link in the email and resets the password.

    - *Alternative 3: user mail does not exist:
        - the system display an error message (your email address does not exist in our system pleas signup)
        - The user clicks the "sign in" button or tray another account.

---
### **Reserving Books**

- **Description**:
    - A user reserves a book that is available for future borrowing.

- **Actors**:
    - User

- **Preconditions**:
    - The user must have a registered account in the system.
    - The book must be available for reservation.

- **Steps**:
    - *Step 1*: The user opens the library system.
    - *Step 2*: The user searches for the book to be reserved.
    - *Step 3*: The user selects the book from the search results.
    - *Step 4*: The user clicks the "Reserve" button.
    - *Step 5*: The system confirms the reservation and displays the reservation expiry date.

- **Alternative Scenarios**:
    - *Alternative 1: Book Not Available for Reservation*:
        - The system displays a message indicating that the book is not available for reservation.

---


## **Book Search**

- **Description**:
- User searches for books in the library system by title, author, genre, or identifier

- **Actors**:
- User

- **Prerequisites**:
- User must have access to the library system.

- **Steps**:
- *Step 1*: User opens the library system.
- *Step 2*: User clicks the "Book Search" page/ pare .
- *Step 3*: User enters search criteria (e.g., title, author, genre, identifier) in the search bar.
- *Step 4*: User clicks the "Search" button.
- *Step 5*: System processes the search query.
- *Step 6*: System displays a list of books that match the search criteria.
- *Step 7*: User selects a book from the search results to view its details.

- **Alternative Scenarios**:
- *Alternative 1: No Matching Results*:
- The system displays a message: "No matching books found."
- The user can modify the search inputs and try again.
---
### **Returning Books**

- **Description**:
    - A user borrows a book from the library and returns it after use.

- **Actors**:
    - User
    - admin 

- **Preconditions**:
    - The user must have a registered account in the system.
  

- **Steps**:
    - *Step 1*: The user returns the book to the library.
    - *Step 2*: The admin scans the book to mark it as returned.
    - *Step 3*: The system updates the user's borrowing history.

- **Alternative Scenarios**:
    - *Alternative 2: Late Return*:
        - The system calculates the overdue fines and displays the amount.

---

### **Managing Overdue Fines**

- **Description**:
    - The system calculates and manages fines for overdue books.

- **Actors**:
    - User

- **Preconditions**:
    - The user must have overdue books.

- **Steps**:
    - *Step 1*: The user logs into the system.
    - *Step 2*: The system checks for overdue books in the user's account.
    - *Step 3*: The system calculates the fine based on the overdue period.
    - *Step 4*: The user pays the fine through the available payment methods.

- **Alternative Scenarios**:
    - *Alternative 1: User Disputes the Fine*:
        - The user contacts library support to resolve the issue.

---

### **Viewing History**

- **Description**:
    - A user views their borrowing and reservation history.

- **Actors**:
    - User
    - admin

- **Preconditions**:
    - The user must have borrowed or reserved books in the past.
  

- **Steps for user **:
    - *Step 1*: The user logs into the system.
    - *Step 2*: The user navigates to the "History" page.
    - *Step 3*: The system displays a list of previously borrowed and reserved books.
- **Steps for admin **:
    - *Step 1*: The admin logs into the system.
    - *Step 2*: The admin navigates to the "History" page.
    - *Step 3*: the admin enter user information .
    - *Step 4*: The system displays a list of previously borrowed and reserved books of this user


---

### **Renew a Book**

- **Description**:
- The user renews a borrowed book to extend the due date.

- **Actors**:
- User

- **Prerequisites**:
- The user must have a borrowed book.
- The book must be eligible for renewal.

- **Steps**:
- *Step 1*: The user logs in to the system.
- *Step 2*: The user goes to the "My Borrowed Books" section.
- *Step 3*: The user selects the book they want to renew.
- *Step 4*: The user clicks the "Renew" button.
- *Step 5*: The system extends the due date and updates the borrowing record.

- **Alternative Scenarios**:
- *Alternative 1: Do Not Allow Renewal*:
- The system displays a message stating that the book is not eligible for renewal (the user cannot borrow the book for 3 weeks (library rules)). 