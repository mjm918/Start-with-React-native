# Start-with-React-native

React-Native works depending on Node.js. Node.js is an open-source, cross-platform JavaScript run-time environment that executes JavaScript code server-side. In mobile development, Node.js helps React-naitve to interact with system APIs.

# Windows
Run `Powershell` with adminstrative permissions and run this to install chocolatey:

`Set-ExecutionPolicy Bypass -Scope Process -Force; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))`

Then run this to install JDK,NodeJS and Python2:
`choco install -y nodejs.install python2 jdk8`

< Troubleshooting >

After installing successfully, check for the environment path. Open cli and type `npm`. If you encounter `npm not recognized` or similar issue, set this `;C:\Program Files\nodejs\` in your environment variable path.

# Mac
If brew is installed, run `brew install node`

Otherwise, download from this link `https://nodejs.org/en/` and follow the installation steps.


# To check the Node.js and NPM version 
`node -v`

`npm -v`

# Install JDK and Android Studio (including all the necessary SDKs)
Install JDK from this link : `http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html`

Install Android Studio with Android SDK from this link: `https://developer.android.com/studio/`

Install XCode from the AppStore for iOS build.

< Troubleshooting >

After installing the JDK, check for Java environment path by typing `java -version` in cli.
If you encounter `java is not recognized` or similar issue, set the jdk path to the environment path variable.

# Installing yarn
`npm i yarn`

Why Yarn? Yarn helps to install Node.js module faster than `npm install`. For example: If you have added new dependencies in your project's `package.json` and want to install or upgrade the new dependencies, you can run `yarn` instead of `npm install`. Another reason is the cli commands are easier than `npm`.

# Installing React Native
`npm install -g react-native-cli`

# Creating React Native projects
`react-native init SampleProject`

# Run the project
To run the app on Android:
`react-native run-android`

To run on iOS:
`react-native run-ios`

This command will run the app on iOS simulator only. If you want to run on physical device, install the following module

`npm install -g ios-deploy`

For OS X 10.11 El Capitan or greater:

`npm install -g ios-deploy --unsafe-perm=true --allow-root`

and then run:

`react-native run-ios --device`
