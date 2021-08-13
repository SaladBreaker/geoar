# Installing

1. `git clone https://github.com/ViroCommunity/geoar.git`
2. `cd geoar`
3. `npm install`
4. `npx pod-install` (iOS)
5. `npx react-native run-android` or `npx react-native run-ios`

# Additional setup

This demo requires a Google Maps Places API key, you can get one from Google Cloud Platform, even it's a paid API Google
offers $200 USD off. After getting a key, set it on the `MAPS_API_KEY` constant on App.js line 25.

# Need help? Or want to contribute?

<a href="https://discord.gg/YfxDBGTxvG">
   <img src="https://discordapp.com/api/guilds/774471080713781259/widget.png?style=banner2" alt="Discord Banner 2"/>
</a>

# Running the project

```shell
npx react-native run-android or npx react-native run-ios
```

```shell
npm start 
```

[comment]: <> (TODO delete this)

# Notes

- error at starting the app try:

```shell
chmod 755 android/gradlew 
```

- android problems

```shell
export ANDROID_SDK_ROOT=/home/vlad/Android/Sdk
```

- adb problems mismatch

```shell
rm /usr/bin/adb
sudo cp /home/vlad/Android/Sdk/platform-tools/adb  /usr/bin/
```

- tcp problem

```shell
adb -s <device> reverse tcp:8081 tcp:8081
