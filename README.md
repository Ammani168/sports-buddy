# Sports Buddy 🏅
Sports Buddy - Admin Dashboard

1. Overview

Sports Buddy is a web application for managing sports events, categories, cities, and areas. The application uses Firebase Firestore for the backend and provides a secure and modular admin dashboard.

2. Features

- Admin login using Firebase Authentication.

- CRUD operations for Sports, Categories, Cities, and Areas.

- Logging for all admin actions.

- Responsive and modular design.

- Firebase Firestore integration.


3. Technologies Used

-> HTML, CSS, JavaScript

-> Firebase (Firestore & Authentication)

GitHub for version control


4. Firebase Setup

-> Create a Firebase project.

-> Enable Firestore Database.

-> Enable Firebase Authentication (Email/Password).

rules_version = '2';
service cloud.firestore {
match /databases/{database}/documents {
match /{document=**} {
allow read, write: if request.auth != null;
}
}
}

5. CRUD Operations

-> Add/Update/Delete Sport

-> Add/Update/Delete Category

-> Add/Update/Delete City

-> Add/Update/Delete Area (Location)


6. Logging

Admin actions are logged in the console and optionally to app.log or Firestore.

7. Deployment

-> Firebase Hosting: firebase init hosting & firebase deploy

-> GitHub: Keep repository public with proper README and workflow documentation.


8. Execution Workflow

- Admin logs in.

- Select module: Sports, Category, City, Area.

- Add/Update/Delete entries.

- Data is stored in Firestore.

- Actions logged.

- Admin views changes in Firebase Console.


9. Set Firestore rules for testing:
  Project Workflow
1. Admin logs in
2. Admin manages sports & locations
3. Users view sports events
4. All actions are logged

5. Deployment
- Firebase Hosting

## How to Run
1. Clone repo
2. Configure Firebase
3. Open index.html


10. Best Practices

- Modular and maintainable code.

- Secure Firebase rules.

- Responsive UI.

- Public GitHub repository for version control.
