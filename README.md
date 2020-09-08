Google Cloud Practice
========================

# 1. Cloud IAM Screenshot 

[here](https://otyo.somanystories.ug/).

<br/>



### Navigate to the root folder of the repo:
$ `cd otyo-mobile-app`

### Install the required dependencies:
$ `npm install`


For reference, this environment variables setup was created based off of this:
https://alxmrtnz.com/thoughts/2019/03/12/environment-variables-and-workflow-in-expo.html





### Expo requirements:

#### Node.js
We recommend the [latest stable version](https://nodejs.org/en/download/), but the maintenance and active LTS releases can also work.

#### Expo client
Expo client is the tool you will use to run your project in development.<br/> 
When you serve your project with Expo CLI, it generates a development URL that you can open in Expo client to preview your app.


*   **If using a phone,**



*  **If using an emulator,**
to run the app directly on your computer, you can find the [iOS simulator instructions here](https://docs.expo.io/versions/v35.0.0/workflow/ios-simulator/) and the [Android emulator instructions here](https://docs.expo.io/versions/v35.0.0/workflow/android-studio-emulator/).<br/> 
The iOS simulator only runs on macOS, Android emulators run on any major operating system.

### Install Expo CLI:
$ `npm install -g expo-cli`


* **Optional: Install Watchman** <br/>
Some macOS users encounter issues if they do not have Watchman installed on their machine, so if you are using a Mac we recommend that you install it. [Download and install Watchman](https://facebook.github.io/watchman/docs/install.html).

### Start the development server:
`npm start`

This will serve the Expo Dev tools on your browser at http://localhost:19002.
The javascript code is bundled and served on port 19001.

### Run the project:
Start the Expo client app on your iOS or Android phone and connect to the same wireless network as your computer.<br/>
On Android, use the Expo app to scan the QR code from your terminal to open your project.<br/>
On iOS, follow on-screen instructions to get a link.

**Congratulations, you are now set.**<br/> 
Now, once you make any changes to the project, the app should auto-reload once you save your changes.<br/>
To debug faster, keep checking the Expo Dev tools, Expo client and the terminal concurrently while working on the project.

## Contribution Guildelines




**NB:** Be VERY careful not to overwrite snapshots with incorrect information. If there's an error due to a snapshot mismatch, first **TRIPLE** check what the issue is rather than just updating the snapshot for the tests to match.

