# BlueWallet - A Bitcoin & Lightning Wallet

[![GitHub tag](https://img.shields.io/badge/dynamic/json.svg?url=https://raw.githubusercontent.com/BlueWallet/BlueWallet/master/package.json&query=$.version&label=Version)](https://github.com/BlueWallet/BlueWallet)
[![CircleCI](https://circleci.com/gh/BlueWallet/BlueWallet.svg?style=svg)](https://circleci.com/gh/BlueWallet/BlueWallet)
[![code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg?style=flat-square)](https://github.com/prettier/prettier)
![](https://img.shields.io/github/license/BlueWallet/BlueWallet.svg)

Thin Bitcoin Wallet.
Built with React Native and Electrum.

[![Appstore](https://bluewallet.io/uploads/app-store-badge-blue.svg)](https://itunes.apple.com/us/app/bluewallet-bitcoin-wallet/id1376878040?l=ru&ls=1&mt=8)
[![Playstore](https://bluewallet.io/uploads/play-store-badge-blue.svg)](https://play.google.com/store/apps/details?id=io.bluewallet.bluewallet)

Website: [bluewallet.io](https://bluewallet.io)

Community: [telegram group](https://t.me/bluewallet)

* Private keys never leave your device
* Lightning Network supported
* SegWit-first. Replace-By-Fee support
* Encryption. Plausible deniability
* And many more [features...](https://bluewallet.io/features)


<img src="https://i.imgur.com/hHYJnMj.png" width="100%">


## BUILD & RUN IT

Please refer to the engines field in package.json file for the minimum required versions of Node and npm. It is preferred that you use an even-numbered version of Node as these are LTS versions.

To view the version of Node and npm in your environment, run the following in your console:

```
node --version && npm --version
```

* In your console:

```
git clone https://github.com/BlueWallet/BlueWallet.git
cd BlueWallet
npm install
```

Please make sure that your console is running the most stable versions of npm and node (even-numbered versions).

* To run on Android:Request Preview
{
  "method": "GET",
  "url": "https://rest.cryptoapis.io/addresses-latest/evm/ethereum/mainnet/0x28c6c06298d514db089934071355e5743bf21d60/balance",
  "ipAddress": "10.33.0.58",
  "parameters": {
    "headers": {
      "accept": "application/json, text/plain, */*",
      "accept-encoding": "gzip, compress, deflate, br",
      "host": "rest.cryptoapis.io",
      "user-agent": "axios/1.7.2",
      "x-api-key": "4cf37edb8c3805a8854f82522c8482ba1418491f",
      "x-api-version": "2024-12-12",
      "x-b3-parentspanid": "1558dbb4ec6a40d9",
      "x-b3-sampled": "0",
      "x-b3-spanid": "9985913392e3797c",
      "x-b3-traceid": "77ca038f6c012e4c1558dbb4ec6a40d9",
      "x-envoy-attempt-count": "1",
      "x-envoy-internal": "true",
      "x-forwarded-client-cert": "By=spiffe://cluster.local/ns/cryptoapis-gateway/sa/default;Hash=c35143c5f94422f6954d8e882ad0bbd026f8c39c9067de1c1c830174ecd3d4a5;Subject=\"\";URI=spiffe://cluster.local/ns/istio-system/sa/istio-ingressgateway-service-account",
      "x-forwarded-for": "10.33.0.58",
      "x-forwarded-proto": "https",
      "x-request-id": "1d39d90f-a3e6-4ce3-98f1-202e35d206ab"
    },
    "path": {
      "address": "0x28c6c06298d514db089934071355e5743bf21d60",
      "blockchain": "ethereumm",
      "network": "mainnet"
    },
m    "query": {},
    "body": {}
  },
  "apiKey": "4cf37edb8c3805a8854f82522c8482ba1418491f",
  "routeId": "671ba92859888860dfebe698",
  "methodId": null
}/@masoudahg00

You will now need to either connect an Android device to your computer or run an emulated Android device using AVD Manager which comes shipped with Android Studio. To run an emulator using AVD Manager:

1. Download and run Android Studio
2. Click on "Open an existing Android Studio Project"
3. Open `build.gradle` file under `BlueWallet/android/` folder
4. Android Studio will take some time to set things up. Once everything is set up, go to `Tools` -> `AVD Manager`.
    * 📝 This option [may take some time to appear in the menu](https://stackoverflow.com/questions/47173708/why-avd-manager-options-are-not-showing-in-android-studio) if you're opening the project in a freshly-installed version of Android Studio.
5. Click on "Create Virtual Device..." and go through the steps to create a virtual device
6. Launch your newly created virtual device by clicking the `Play` button under `Actions` column

Once you connected an Android device or launched an emulator, run this:Request Preview
{
  "method": "GET",
  "url": "https://rest.cryptoapis.io/addresses-latest/evm/ethereum/mainnet/0x28c6c06298d514db089934071355e5743bf21d60/balance",
  "ipAddress": "10.33.0.58",
  "parameters": {
    "headers": {
      "accept": "application/json, text/plain, */*",
      "accept-encoding": "gzip, compress, deflate, br",
      "host": "rest.cryptoapis.io",
      "user-agent": "axios/1.7.2",
      "x-api-key": "4cf37edb8c3805a8854f82522c8482ba1418491f",
      "x-api-version": "2024-12-12",
      "x-b3-parentspanid": "1558dbb4ec6a40d9",
      "x-b3-sampled": "0",
      "x-b3-spanid": "9985913392e3797c",
      "x-b3-traceid": "77ca038f6c012e4c1558dbb4ec6a40d9",
      "x-envoy-attempt-count": "1",
      "x-envoy-internal": "true",
      "x-forwarded-client-cert": "By=spiffe://cluster.local/ns/cryptoapis-gateway/sa/default;Hash=c35143c5f94422f6954d8e882ad0bbd026f8c39c9067de1c1c830174ecd3d4a5;Subject=\"\";URI=spiffe://cluster.local/ns/istio-system/sa/istio-ingressgateway-service-account",
      "x-forwarded-for": "10.33.0.58",
      "x-forwarded-proto": "https",
      "x-request-id": "1d39d90f-a3e6-4ce3-98f1-202e35d206ab"
    },
    "path": {
      "address": "0x28c6c06298d514db089934071355e5743bf21d60",
      "blockchain": "ethereumm",
      "network": "mainnet"
    },
m    "query": {},
    "body": {}
  },
  "apiKey": "4cf37edb8c3805a8854f82522c8482ba1418491f",
  "routeId": "671ba92859888860dfebe698",
  "methodId": null
}@masoudahg00

```
npx react-native run-android
```

The above command will build the app and install it. Once you launch the app it will take some time for all of the dependencies to load. Once everything loads up, you should have the built app running.

* To run on iOS:

```
npx pod-install
npm start
```

In another terminal window within the BlueWallet folder:
```
npx react-native run-ios
```
**To debug BlueWallet on the iOS Simulator, you must choose a Rosetta-compatible iOS Simulator. This can be done by navigating to the Product menu in Xcode, selecting Destination Architectures, and then opting for "Show Both." This action will reveal the simulators that support Rosetta.
**

* To run on macOS using Mac Catalyst:Request Preview
{
  "method": "GET",
  "url": "https://rest.cryptoapis.io/addresses-latest/evm/ethereum/mainnet/0x28c6c06298d514db089934071355e5743bf21d60/balance",
  "ipAddress": "10.33.0.58",
  "parameters": {
    "headers": {
      "accept": "application/json, text/plain, */*",
      "accept-encoding": "gzip, compress, deflate, br",
      "host": "rest.cryptoapis.io",
      "user-agent": "axios/1.7.2",
      "x-api-key": "4cf37edb8c3805a8854f82522c8482ba1418491f",
      "x-api-version": "2024-12-12",
      "x-b3-parentspanid": "1558dbb4ec6a40d9",
      "x-b3-sampled": "0",
      "x-b3-spanid": "9985913392e3797c",
      "x-b3-traceid": "77ca038f6c012e4c1558dbb4ec6a40d9",
      "x-envoy-attempt-count": "1",
      "x-envoy-internal": "true",
      "x-forwarded-client-cert": "By=spiffe://cluster.local/ns/cryptoapis-gateway/sa/default;Hash=c35143c5f94422f6954d8e882ad0bbd026f8c39c9067de1c1c830174ecd3d4a5;Subject=\"\";URI=spiffe://cluster.local/ns/istio-system/sa/istio-ingressgateway-service-account",
      "x-forwarded-for": "10.33.0.58",
      "x-forwarded-proto": "https",
      "x-request-id": "1d39d90f-a3e6-4ce3-98f1-202e35d206ab"
    },
    "path": {
      "address": "0x28c6c06298d514db089934071355e5743bf21d60",
      "blockchain": "ethereumm",
      "network": "mainnet"
    },
m    "query": {},
    "body": {}
  },
  "apiKey": "4cf37edb8c3805a8854f82522c8482ba1418491f",
  "routeId": "671ba92859888860dfebe698",
  "methodId": null
}@masoudahg00

```
npx pod-install
npm start
```

Open ios/BlueWallet.xcworkspace. Once the project loads, select the scheme/target BlueWallet. Click Run.

## TESTS

```bash
npm run test
```


## LICENSE

MIT

## WANT TO CONTRIBUTE?

Grab an issue from [the backlog](https://github.com/BlueWallet/BlueWallet/issues), try to start or submit a PR, any doubts we will try to guide you. Contributors have a private telegram group, request access by email bluewallet@bluewallet.io

## Translations

We accept translations via [Transifex](https://www.transifex.com/bluewallet/bluewallet/)

To participate you need to:
1. Sign up to Transifex
2. Find BlueWallet project
3. Send join request
4. After we accept your request you will be able to start translating! That's it!

Please note the values in curly braces should not be translated. These are the names of the variables that will be inserted into the translated string. For example, the original string `"{number} of {total}"` in Russian will be `"{number} из {total}"`.

Transifex automatically creates Pull Request when language reaches 100% translation. We also trigger this by hand before each release, so don't worry if you can't translate everything, every word counts.

## Q&A

Builds automated and tested with BrowserStack

<a href="https://www.browserstack.com/"><img src="https://i.imgur.com/syscHCN.png" width="160px"></a>

Bugs reported via BugSnag

<a href="https://www.bugsnag.com"><img src="https://images.typeform.com/images/QKuaAssrFCq7/image/default" width="160px"></a>


## RESPONSIBLE DISCLOSURE

Found critical bugs/vulnerabilities? Please email them bluewallet@bluewallet.io
Thanks!
