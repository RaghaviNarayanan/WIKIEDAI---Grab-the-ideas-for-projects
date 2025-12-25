# WIKIEDAI---Grab-the-ideas-for-projects
WikiEDAI is a mobile application developed to help engineering students find suitable project ideas easily. The main purpose of this project is to provide a single platform where users can browse, explore, and contribute engineering project ideas across different technical domains. The application is built using Flutter for the frontend and Firebase for backend services.

When the application is opened, the user is shown a home screen where different project domains are displayed. The user can browse through these domains and view a list of available project ideas. Each project contains details such as the project title, description, domain, and contributor information. This allows students to quickly understand the idea and decide whether it matches their interests.

If a user wants to add a new project idea, they can do so directly from the application. The user enters the project details such as title, description, selected domain, and contact information. Before submission, the application checks whether all required fields are filled correctly. Once validated, the project information is sent to Firebase Firestore, where it is stored as structured data.

If the project includes images or related files, they are uploaded separately to Firebase Storage. After the upload is completed, Firebase generates a secure link for the file, which is then saved along with the project details in Firestore. This separation of data and files ensures smooth performance and efficient storage.

Whenever a user browses or searches for projects, the application fetches data directly from Firebase Firestore. Real-time listeners are used so that any newly added project appears instantly in the app without requiring a refresh. Images are loaded only when needed, which reduces data usage and improves responsiveness.

Overall, the flow of the project starts with user interaction on the Flutter application, followed by data validation, cloud storage using Firebase, and real-time retrieval of project information. This flow makes WikiEDAI a reliable, scalable, and user-friendly platform for discovering and sharing engineering project ideas.
