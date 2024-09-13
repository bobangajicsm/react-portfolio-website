# React-portfolio-website

## Getting Started

### Prerequisites

Make sure you have Node.js and npm installed on your machine. You can download them from [Node.js](https://nodejs.org/).

### Installation

1. **Clone the repository**  
   Clone the project to your local machine using Git:

   ```bash
   git clone https://github.com/bobangajicsm/react-portfolio-website.git
   cd react-portfolio-website
   ```

2. **Install dependencies**  
   After cloning, you need to install the required npm packages. Run:

   ```bash
   npm install
   ```

   This will install all necessary dependencies mentioned in `package.json`.

3. **Firebase Setup**  
   To integrate Firebase into your project, follow the steps below:

   - **Create a Firebase Account**  
     Go to [Firebase](https://firebase.google.com) and log in or create a new account.

   - **Create a New Project**  
     Click on "Add Project" and follow the on-screen instructions to create a new Firebase project.

   - **Register Your Web App**  
     After creating the project, select "Web" as the platform, and register your web app. Firebase will generate a configuration object for you.

   - **Install Firebase SDK**  
     Run the following command to install Firebase SDK:

     ```bash
     npm install firebase
     ```

   - **Edit `firebase.js`**  
     In your project directory, create a file named `firebase.js` and update it with your Firebase config:

     ```javascript
     // firebase.js
     import { initializeApp } from "firebase/app";

     const firebaseConfig = {
       apiKey: "YOUR_API_KEY",
       authDomain: "YOUR_AUTH_DOMAIN",
       projectId: "YOUR_PROJECT_ID",
       storageBucket: "YOUR_STORAGE_BUCKET",
       messagingSenderId: "YOUR_MESSAGING_SENDER_ID",
       appId: "YOUR_APP_ID"
     };

     const app = initializeApp(firebaseConfig);

     export default app;
     ```

   Replace the placeholder values with your actual Firebase configuration.

4. **Run the App**  
   To start the app in development mode, run:

   ```bash
   npm start
   ```

   This will open the app in your default browser at [http://localhost:3000](http://localhost:3000). The app will reload automatically when you make changes to the code.

### Building for Production

To build the app for production:

```bash
npm run build
```

This will create a production-ready build of the app in the `build` folder.

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

The page will reload automatically if you make changes to the code. You may also see any lint errors in the console.

### `npm run build`

Builds the app for production to the `build` folder.\
It bundles React in production mode and optimizes the build for the best performance. The build is minified, and filenames include the hashes. Your app is ready to be deployed.

### `npm run eject`

If you want to customize the build configuration and dependencies, you can run:

```bash
npm run eject
```

**Note:** This is a one-way operation. Once you eject, you can’t go back!

### Testing

To run tests in watch mode:

```bash
npm test
```

## Learn More

You can learn more about Create React App and Firebase from the following resources:

- [Create React App Documentation](https://facebook.github.io/create-react-app/docs/getting-started)
- [Firebase Documentation](https://firebase.google.com/docs/web/setup)
- [React Documentation](https://reactjs.org/)

```
