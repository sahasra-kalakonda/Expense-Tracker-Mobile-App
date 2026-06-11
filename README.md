# My Expense Tracker
 
A React Native mobile app built with Expo for tracking personal expenses. View recent expenses, browse all-time history, and add or edit entries   ~ all in a clean, intuitive interface.
 
## Screenshots
 
> Add screenshots of your app here.
 
## Features
 
- **Recent Expenses** — View expenses from the last 7 days at a glance
- **All Expenses** — Browse your full expense history
- **Add / Edit / Delete** — Manage expenses through a modal screen
- **Context API** — Lightweight global state management (no Redux needed)
- **Bottom Tab Navigation** — Fast switching between Recent and All views
- **Modal Stack Navigation** — Smooth UX for adding and editing entries

## Tech Stack
 
| Technology | Version |
|---|---|
| React Native | 0.73.6 |
| Expo | ~50.0.17 |
| React Navigation (Native Stack) | ^6.9.26 |
| React Navigation (Bottom Tabs) | ^6.5.20 |
| Expo Font | ~11.10.3 |
| Expo Linear Gradient | ~12.7.2 |
 
## Project Structure
 
```
├── App.js                  # Root component, navigation setup
├── app.json                # Expo configuration
├── babel.config.js         # Babel configuration
├── eas.json                # EAS Build configuration
├── assets/                 # App icons, splash screen
├── screens/
│   ├── ManageExpense.js    # Add / Edit / Delete expense screen
│   ├── RecentExpenses.js   # Last 7 days view
│   └── AllExpenses.js      # Full history view
├── components/
│   └── UI/
│       └── IconButton.js   # Reusable icon button component
├── constants/
│   └── styles.js           # Global color palette and styles
└── store/
    └── expenses-context.js # React Context for expense state
```
 
## Getting Started
 
### Prerequisites
 
- [Node.js](https://nodejs.org/) (v18+)
- [Expo CLI](https://docs.expo.dev/get-started/installation/)
- Expo Go app on your iOS or Android device (for local testing)
### Installation
 
```bash
# Clone the repository
git clone https://github.com/your-username/my-expense-tracker.git
cd my-expense-tracker
 
# Install dependencies
npm install
 
# Start the development server
npm start
```
 
Then scan the QR code with Expo Go (Android) or the Camera app (iOS).
 
### Running on a specific platform
 
```bash
# Android
npm run android
 
# iOS
npm run ios
 
# Web
npm run web
```
 
## Building for Production
 
This project uses [EAS Build](https://docs.expo.dev/build/introduction/).
 
```bash
# Install EAS CLI
npm install -g eas-cli
 
# Log in to your Expo account
eas login
 
# Build for Android (APK preview)
eas build --platform android --profile preview
 
# Build for production
eas build --platform all --profile production
```
 
---
 
## ⚙️ Configuration
 
App settings are managed in `app.json`:
 
| Setting | Value |
|---|---|
| App Name | My Expense Tracker |
| Bundle ID (Android) | `com.sahasrakalakonda.myexpensetracker` |
| Orientation | Portrait |
| EAS Project ID | `8eccf8fd-ebe6-4bb9-8558-1be91de823df` |
 
---
 
## Theming
 
Colors are defined in `constants/styles.js` via `GlobalStyles.colors`. The app uses a purple/indigo primary palette with an amber accent.
 
---
 
## 📄 License
 
This project is for personal/educational use. Feel free to fork and adapt it.
