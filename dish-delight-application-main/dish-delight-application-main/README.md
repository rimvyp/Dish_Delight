# Dish Delight

React Native (Expo) frontend with example Express + Firebase Admin code used during development.

## Quick summary
- Frontend: Expo / React Native app. Entry: `App.js`.
- API client: `Firebase/client.js`  functions for register/login, fetching meals, recipes, favourites.
- Example backend: `Firebase/server.js` and `Firebase/ServerVM.js` (Express + Firebase Admin).
- Screens: `src/` contains Login, Register, Home (FourButtonScreen), Meals, Steps, Favorites, Reviews, About.

## Project layout (important files)
- App.js  app entry and navigation
- package.json  project scripts and dependencies
- src/  UI screens
  - FourButtonScreen.js, Login.js, RegisterScreen.js, MealsScreen.js, AllRecipes.js, FavoritesScreen.js, ReviewScreen.js, AboutScreen.js
  - Meals/ and Steps/  example recipe pages
- Firebase/
  - client.js  frontend API client (points to the server IP)
  - server.js, ServerVM.js  example Express servers that use Firestore via Firebase Admin
  - finished/  contains a Firebase service account JSON (sensitive)

## Run (frontend)
1. Open repository folder (same folder as `package.json`):
   - npm install
   - npm run start
   - Use Expo to open on simulator or device
2. If using a physical device, set the server IP in `Firebase/client.js` (replace `localhost` with your machine IP).

## Run (example backend)
1. cd `Firebase`
2. npm install
3. node server.js  (or `node ServerVM.js`)
4. Server listens on port 3000 by default


