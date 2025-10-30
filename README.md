# Unwiind

A React Native mobile application for music streaming, social interaction, and content sharing. Built with Expo and Firebase.

## 📱 About

Unwiind is a multi-platform mobile application that combines music streaming with social features like forums, chat, and content sharing. The app provides a seamless experience for discovering and enjoying media content while connecting with other users.

## ✨ Features

- **Music Player** - Stream and play audio content with full playback controls
- **User Authentication** - Secure login and account creation with Firebase
- **Social Features**
  - Private chat messaging
  - Forum discussions
  - Thread-based conversations
- **Content Management**
  - Media library with multiple views
  - Favorites and recent history
  - Profile customization
- **Redux State Management** - Persistent app state across sessions
- **Multi-platform Support** - iOS, Android, and Web

## 🛠 Tech Stack

- **Framework**: React Native 0.63.4 with Expo SDK 41
- **Navigation**: React Navigation 5.x (Stack & Bottom Tabs)
- **State Management**: Redux with Redux Saga & Redux Persist
- **Backend**: Firebase 8.2.3
- **UI Components**: NativeBase 2.15.2
- **Media**: Expo AV for audio/video playback
- **Authentication**: Expo Google Sign-In

## 📋 Prerequisites

Before you begin, ensure you have the following installed:

- [Node.js](https://nodejs.org/) (v12 or higher)
- [npm](https://www.npmjs.com/) or [yarn](https://yarnpkg.com/)
- [Expo CLI](https://docs.expo.dev/get-started/installation/)
- [React Native CLI](https://reactnative.dev/docs/environment-setup)
- Android Studio (for Android development)
- Xcode (for iOS development, macOS only)

## 🚀 Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/superdev947/unwinnd.git
   cd unwinnd
   ```

2. **Install dependencies**
   ```bash
   npm install
   # or
   yarn install
   ```

3. **Configure Firebase**
   - Create a Firebase project at [Firebase Console](https://console.firebase.google.com/)
   - Add your `google-services.json` file to the root directory (for Android)
   - Update Firebase configuration in `src/constants/firebase.js`

## 🏃‍♂️ Running the App

### Development Mode

**Start Metro bundler:**
```bash
npm start
# or
react-native start
```

**Run on Android:**
```bash
npm run android
# or
react-native run-android
```

**Run on iOS:**
```bash
npm run ios
# or
react-native run-ios
```

**Run on Web:**
```bash
npm run build:web
```

## 📁 Project Structure

```
unwinnd/
├── src/
│   ├── assets/              # Images, fonts, and static resources
│   ├── components/          # Reusable UI components
│   ├── constants/           # App constants (colors, layouts, Firebase config)
│   ├── navigation/          # Navigation configuration
│   │   ├── Guest.js         # Guest user navigation
│   │   └── Logged.js        # Authenticated user navigation
│   ├── redux/               # State management
│   │   ├── Store.js         # Redux store configuration
│   │   ├── actions/         # Redux actions
│   │   ├── reducers/        # Redux reducers
│   │   └── services/        # API services
│   └── screens/             # App screens
│       ├── Guest/           # Pre-authentication screens
│       │   ├── CreateAccount.js
│       │   └── Login.js
│       └── Logged/          # Post-authentication screens
│           ├── ChatPrivate.js
│           ├── ChatThread.js
│           ├── Content.js
│           ├── Favorites.js
│           ├── Forum.js
│           ├── Media1.js
│           ├── Media2.js
│           ├── Media3.js
│           ├── Player.js
│           ├── Profile.js
│           ├── Recent.js
│           └── Unwiind.js
├── App.js                   # Main app component
├── index.js                 # Entry point
├── app.json                 # Expo configuration
├── package.json             # Dependencies
└── babel.config.js          # Babel configuration
```

## 🏗 Building for Production

### Android

```bash
npm run build
# or
expo build:android
```

### iOS

```bash
npm run build:ios
# or
expo build:ios
```

### Generate Android Fingerprint

```bash
npm run build:fingerprint
```

## 🔧 Configuration

### Firebase Setup

Update the Firebase configuration in `src/constants/firebase.js` with your project credentials:

```javascript
const firebaseConfig = {
  apiKey: "YOUR_API_KEY",
  authDomain: "YOUR_AUTH_DOMAIN",
  projectId: "YOUR_PROJECT_ID",
  storageBucket: "YOUR_STORAGE_BUCKET",
  messagingSenderId: "YOUR_MESSAGING_SENDER_ID",
  appId: "YOUR_APP_ID"
};
```

### App Configuration

Modify `app.json` to customize:
- App name and slug
- Bundle identifiers
- Version numbers
- Icons and splash screens
- Orientation and platform settings

## 📦 Dependencies

### Key Dependencies

- `react-native` - Core framework
- `expo` - Development platform
- `@react-navigation` - Navigation library
- `redux`, `react-redux`, `redux-saga` - State management
- `firebase` - Backend services
- `native-base` - UI component library
- `expo-av` - Audio/video playback
- `@react-native-async-storage/async-storage` - Local storage

See `package.json` for the complete list of dependencies.

## 🧪 Testing

```bash
npm test
```

## 📱 App Versions

- **Current Version**: 1.1.4
- **iOS Build**: 1.1.4
- **Android Version Code**: 1

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is private and proprietary.

## 👤 Author

**superdev947**

- GitHub: [@superdev947](https://github.com/superdev947)

## 📞 Support

For support, please open an issue in the GitHub repository.

---

Made with ❤️ using React Native and Expo
