![Architecture](https://raw.githubusercontent.com/origreen/.github/main/profile/logo.png)

# Origreen - A green origin!

## Try it!!!

**URL TO THE PROFILATION**: https://origreen.vercel.app/

**URL TO THE DETAILS OF A FOOD**: https://origreen.vercel.app/food/white_cabbage

**You will notice that changing the parameters in the profilation will result in a different score in the details page!**

**If you want to use the api, follow [this link](https://origreen-apis.herokuapp.com/food/white_cabbage)**

## How was it made

- A backend with **Python** and **FastAPI**
- A webapp with **Vue.js**
- An app with **Unity**
- A database with **MongoDB**


### The database model

The database contains two collections:
- __food__: all the possible food, with all the information about how and where it grew (the qrcodes contain the id of the db record)
- __profiles__: a score is calculated to say if the food is suggested. There can be profilation on this, so some users can be interested in some aspects and other students in other aspects. These _weights__ of profilations are stored in this collection

### The backend

The backend:
- Serves the DB data
- Calculates the score of a food based on the weights
- Allow to select a predefined weights-profile or to add a custom one

### The webapp

- It allows you to change the weights
- It shows the in-detail information about a certain food

### The app

- Scans the QRCodes and shows the score with AR
- When the QRCode is clicked, it takes the user to the webapp to see more information

## Architecture

![Architecture](https://raw.githubusercontent.com/origreen/.github/main/profile/architecthure.png)
