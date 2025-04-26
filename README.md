# PharmaCheck Telegram APP

## Overview

The project consists of a `Telegram Bot Authentication System`, a `Prescription API Service`, and a `Frontend Application` built using React. The project allows users to interact with the system via Telegram for authentication and provides prescription services through a web-based application.

## 1. Telegram Bot Authentication Server

### Purpose

The server handles authentication for users via a [Telegram bot](https://github.com/Gozkybrain/Telegram-Node-Auth). The bot interacts with the users, gathers their credentials [username and userID], and sends them to the backend to authenticate users for the application.

The tech stack for this part is Node.js, Express.js, and Firebase (for storing user information as database).

### Bot Workflow

* User interacts with Telegram bot (`@PharmaCheckBot`).
* The user clicks on `Start` button and the bot replies with an authentication status.
* The message contains the Dashboard link and a link to check the server status.
* The user can then open their dashboard on the app and they are authenticated with their username.

## 2. Prescription API Service

### Purpose
The  [Prescription API](https://github.com/Gozkybrain/Pharma-Check) provides medical prescriptions based on the user's input. It serves this data to the frontend app, allowing users to search for and receive medication information.

Tech stack needed for this part are Node.js and Express.js.


### Data Sample
<pre> {
    "id": "1",
    "name": "Amoxicillin",
    "description": "Amoxicillin is used to treat a wide variety of bacterial infections.",
    "sideEffects": [
      "Nausea",
      "Vomiting"
    ],
    "category": "Antibiotic",
    "treatment": [
      "Bacterial infections"
    ],
    "minAge": 0
  },
</pre>


## 3. Frontend Application

The frontend application is built using React and provides an interface for users to interact with the prescription data, log in via Telegram authentication, and access the dashboard.

### Future Upgrades
* Doctor's page where user can explain their symptoms.
* A standard user dashboard for users to manage
