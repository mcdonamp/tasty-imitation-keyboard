
# Tasty Imitation Keyboard + Firebase Keylogger

This is based on the [Tasty Imitation Keyboard](https://github.com/archagon/tasty-imitation-keyboard), and shows how to integrate [Firebase Authentication](https://firebase.google.com/docs/auth/), [Realtime Database](https://firebase.google.com/docs/database/), and [Storage](https://firebase.google.com/docs/storage/) to make a super simple keylogger + screenshot taker.

** Note ** This is so hilariously against Apple's ToS that I recommend using it only so far as to see how to set up a custom keyboard extension to use Firebase, then removing the additional functionality. I guarantee that if you try to ship this to the App Store, the app will get rejected and your account may get banned. Just don't do it.

## Special Bonus Firebase Features

* Logs individual keypresses to the Firebase Realtime Database
* Screenshots individual keypresses and saves the images to Firebase Storage
* Authenticates a user anonymously

## Build Instructions

0. [Create a new free Firebase project](https://console.firebase.google.com) and create a new iOS App.
0. Download the `GoogleService-Info.plist` and replace the included one with your downloaded copy. Make sure to click "copy if necessary" since, yes, it is necessary.
0. `pod install` and open `TastyImitationKeyboard.xcworkspace`
1. Edit Scheme for the `Keyboard` target and set the Executable to be `HostingApp.app`.
2. Run the `Keyboard` target.
3. Go to `Settings → General → Keyboard → Keyboards → Add New Keyboard` on your device and add the third-party keyboard.
4. Go back to the app. You should be able to select the keyboard via the globe icon.
5. ???
6. Profit!

## License

This project is licensed under the 3-clause ("New") BSD license. Go Bears!
