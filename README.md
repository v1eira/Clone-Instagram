# Clone-Instagram
An Instagram-like app

## Environment
- OS: [Ubuntu 18.04](http://releases.ubuntu.com/18.04/)
- Node.js v10.x: <br>
    `` $ curl -sL https://deb.nodesource.com/setup_10.x | sudo -E bash - `` <br>
    `` $ sudo apt-get install -y nodejs ``
- Yarn: <br>
    `` $ curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add - ``

    `` $ echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list ``

    `` $ sudo apt update `` <br>
    `` $ sudo apt install --no-install-recommends yarn `` <br>

- Insomnia: <br>
    `` # Add to sources `` <br>
    `` $ echo "deb https://dl.bintray.com/getinsomnia/Insomnia /" \ `` <br>
    `` $ | sudo tee -a /etc/apt/sources.list.d/insomnia.list ``

    `` # Add public key used to verify code signature `` <br>
    `` $ wget --quiet -O - https://insomnia.rest/keys/debian-public.key.asc \ `` <br>
    `` $ | sudo apt-key add - ``

    `` # Refresh repository sources and install Insomnia `` <br>
    `` $ sudo apt-get update `` <br>
    `` $ sudo apt-get install insomnia ``

## Tools
Inside the backend folder:
- `` $ yarn add express ``
- `` $ yarn add mongoose ``
- `` $ yarn add sharp ``
- `` $ yarn add cors ``

Inside the frontend folder:
- `` $ yarn add react-router-dom ``
- `` $ yarn add socket.io-client ``

I used my phone to emulate the app, so:
- `` $ npm install -g react-native cli ``
- `` $ yarn add react-navigation react-native-gesture-handler ``
- `` $ react-native link react-native-gesture-handler ``
- `` $ react-native run-android ``

To use the camera on Android:
- `` $ yarn add react-native-image-picker ``
- `` $ react-native link react-native-image-picker ``
- Then, follow [this](https://github.com/react-native-community/react-native-image-picker/blob/master/docs/Install.md)

## Running the app:
Start the server on the ``backend`` folder: <br>
``$ yarn dev``

Run the frontend at the ``frontend`` folder: <br>
``$ yarn start``

To run the mobile version, go to the ``instarocket`` folder and do: <br>
``$ react-native run-android``

Here is how it looks:

#### Web

![frontend-feed](/img/frontend-feed.png) <br><br>

![frontend-new](/img/frontend-new.png) <br><br>

#### Mobile

![mobile-feed](/img/mobile-feed.jpg) <br><br>

![mobile-new](/img/mobile-new.jpg)