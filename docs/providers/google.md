## Google provider implementation

[Go back to README](../../README.md)

- Start with installation steps on [README page](../../README.md).
- **Install required package via npm:**

(Don't be confused by google-plus in package name, package already uses new Google API, not deprecated Google Plus API)
```bash
npm install @ionic-native/google-plus
```

- **Go to Firebase → select your project → Authentication → Sign-in method
→ Google → Enable → Choose your support email → Save**

- Go to [Google APIs Console → Credentials](https://console.developers.google.com/apis/credentials/).
Select a different project at the top on left side if needed (select All in project select popup).

- In OAuth 2.0 Client IDs section select Web client and copy Client ID and use it in next step.

- Install cordova module package via npm:

(Change WEB_APPLICATION_CLIENT_ID variable to your Client ID (Web client) from Google APIs Console - previous step)
```bash
ionic cordova plugin add cordova-plugin-googleplus --variable WEB_APPLICATION_CLIENT_ID="xxx.apps.googleusercontent.com"
```

## Usage

See [example project](https://github.com/cothema/ionic-firebase-login-tutorial)

## Frequent errors

- **Error: Uncaught (in promise): 10**
  - You don't have sign your app correctly or you have wrong client id in your configuration.

