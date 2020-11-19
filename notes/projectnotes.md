<h1 align="center">
Solo React Project Steps
</h1>


1. This repo has the backend and frontend - All the npm packages you need are already installed.

2. Make sure you "npm install" in the root of the folder - this will install all the dependacies for the backend.

3. All the Frontend is inside the client folder - CD into it and npm install (this will install all the react npm packages)

4. You are now ready to start

5. In order to connect the frontend with the backend you have to "npm start" on both the root directory and cd into the "client" folder and "npm start" there too. Don't worry about doing it now. You have to setup the DB first. They are two seperate things and need to both be on to talk to each other.

6. Let me try and explain some shit first. Idk if I'm 100% sure so take what I say with a grain of salt.

7. Dont touch anything on the ./bin/www file - remember the bin folder is a common Unix convention for naming a folder that contains executable code. Even though it is lacking the .js file extension, the www file is actually a JS module that contains code to start up the express app.

8. Since your app will use a database for data persistence your project needs to include a way to configure the database connection settings across environments. To do that, let's use environment variables to configure the app.

9. As a reminder the 'per-env' package (It's already installed) allows you to define npm scripts for each of your apps environment. The 'dotenv' package (It's already installed) is used to load environment variables from the .env file and the 'dotenv-cli' (It's already installed) package acts as an intermediary between npx and tools or utilities (like the sequelize cli) to load your environment variables from an .env fila and run the command that you pass into it.
