# SCHEDJ Frontend
[![Build](https://travis-ci.com/Schedj/schedj-frontend.svg?branch=master)](https://travis-ci.com/Schedj/schedj-frontend)
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)

A mobile application for students to access and manage scheduling and student accounts. Utilizes React Native to cross-platform deploy. Connects to the SCHEDJ backend for API and data.

## Installation
We use the Expo SDK currently. Make sure you have the latest version of [node.js](https://nodejs.org/en/) installed on your computer. Then, open a terminal and browse to your working directory, and run the following:
```
git clone https://github.com/Schedj/schedj-frontend
cd schedj-frontend
npm install
```
This will install the Expo CLI. Check out the docs for Expo [here](https://expo.io/tools).

Before running, we need to go into the main repository and create a file `env.js` with the template below, but change the `server_ip` section to your computer's [public ip](https://www.whatismyip.com/what-is-my-public-ip-address/) (IPv4). This can be found in a number of ways. Setting `local` to true works for on-device emulators (such as macOS's Simulator or the Android Emulator).
```
export default {
   server: {
      local: false,
      server_ip: '123.456.789.876',
      port: '8080'
   }
}
```

Then, run `npm start`. This will start the Expo server. The docs for Expo can be found [here](https://docs.expo.io/versions/latest/).
