# Mobile UI testing with React Native and Maestro

## Introduction


I created a React Native app built with Expo to simply this part. The aim of this project is `Maestro`.
Enjoy it! :)

This app has three screens:

- A sign in interface with two fields, email and password. After clicking the sign in button, if the form is valid `(a valid email and password)` we'll see the next screen.
- A simple screen with greetings and email user, a link to another screen and a sign out button.
- A scrollview screen with some texts and images. It's also possible to go back to the previous screen.

<img src="./docs/app.gif" alt="React Native Maestro app" />

## Installation

### React Native Maestro

```shell
$ git clone https://github.com/kiki-le-singe/react-native-maestro.git <name>
$ cd <name>
$ npm install
```

### Maestro

```shell
$ curl -Ls "https://get.maestro.mobile.dev" | bash
$ maestro -v
```

> Only for iOS: [Connecting to Your Device](https://maestro.mobile.dev/getting-started/installing-maestro#connecting-to-your-device)

```shell
$ brew tap facebook/fb
$ brew install facebook/fb/idb-companion
```

See the official documentation: [Installing Maestro](https://maestro.mobile.dev/getting-started/installing-maestro)

## Run

```bash
$ npm start
$ npm run ios or android
```

## Maestro tests

The tests are in the `maestro` directory. You can run them locally in your iOS simulator or Android emulator. At the moment, Maestro does not support real iOS devices. See [Installing Maestro](https://maestro.mobile.dev/getting-started/installing-maestro) and [Connecting to Your Device](https://maestro.mobile.dev/getting-started/installing-maestro#connecting-to-your-device)

You can run the tests in CI with `Maestro Cloud`. See [Running Flows on CI](https://maestro.mobile.dev/getting-started/running-flows-on-ci).

### Running tests

```bash
# run single test
$ maestro test maestro/[fileName].yaml
```

<br />

```bash
$ maestro test maestro/simple-flow.yaml
```

<img src="./docs/simple-maestro-flow.gif" alt="Simple Maestro flow" width="800" height="600" />

<br /><br />

```bash
$ maestro test maestro/signin/signin-errors-flow.yaml
```

<img src="./docs/signin-errors-flow.gif" alt="Sign in errors Maestro flow" width="800" height="600" />

<br /><br />

```bash
$ maestro test maestro/signin/signin-success-flow.yaml
```

<img src="./docs/signin-success-flow.gif" alt="Sign in success Maestro flow" width="800" height="600" />

<br /><br />

```bash
$ maestro test maestro/home/home-flow.yaml
```

<img src="./docs/home-flow.gif" alt="Home flow" width="800" height="600" />

<br /><br />

```bash
$ maestro test maestro/details/details-flow.yaml
```

<img src="./docs/details-flow.gif" alt="Details flow" width="800" height="600" />

<br />

> Sometimes you could see this error: [Failed to reach out XCUITest Server](https://github.com/mobile-dev-inc/maestro/issues/880)... Maybe your component is not reachable, so you probably check your code. Sometimes the CLI just seems a little capricious... So just wait a few secondes... And it perfectly works! :D


#   m i d a s - r e a c t _ n a t i v e _ a p p 
 
 
