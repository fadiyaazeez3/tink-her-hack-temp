<p align="center">
  <img src="./img.png" alt="Project Banner" width="100%">
</p>

# WALKGUARD 🎯

## Basic Details

### Team Name: LEAD

### Team Members
- Member 1: Fadiya Azeez - Bharata Mata College, Thrikkakara
- Member 2: Aiswarya Asokan - Bharata Mata College, Thrikkakara

### Hosted Project Link
[mention your project hosted link here]

### Project Description
This project is a mobile safety application that allows users to send instant SOS alerts with their live location to saved emergency contacts. It also includes a background tracking feature that can share real-time location updates for added safety. The app is designed as a quick-response personal security tool, especially useful in emergency or unsafe situations.

### The Problem statement
Many people, especially women and individuals traveling alone, face unsafe situations where they cannot quickly contact help. Existing emergency solutions are slow, complicated, or require multiple steps during panic situations. There is a need for a fast, simple, and reliable emergency alert system that instantly shares location and distress signals.

### The Solution
This app provides a one-tap SOS system that immediately sends emergency messages with live GPS location to saved contacts. It also includes a background tracking mode that continuously monitors location for safety monitoring. The solution is designed to work quickly, require minimal interaction, and function even when the user cannot manually type or call.

---

## Technical Details

### Technologies/Components Used

**For Software:**
- Languages used: JavaScript
- Frameworks used: React Native, Expo
- Libraries used: expo-location → GPS access, expo-sms → SMS sending,expo-task-manager → background tracking, AsyncStorage → local data storage
- Tools used: VS Code (code editor), Node.js (runtime), Expo CLI (app runner), Git (version control)

**For Hardware:**
- Main components: Android smartphone
- Specifications: GPS enabled device, SMS capability

---

## Features

List the key features of your project:
- Feature 1: SOS Emergency Button (Sends instant emergency SMS with live location).
- Feature 2: Contact Storage (Saves emergency numbers locally using AsyncStorage).
- Feature 3: Background Tracking Mode (Tracks user location continuously for safety monitoring).
- Feature 4: Real-time Location Link (Sends clickable Google Maps link in SOS message).

---

## Implementation

### For Software:

#### Installation
```bash
npm install
npx expo install expo-location expo-sms expo-task-manager @react-native-async-storage/async-storage
```

#### Run
```bash
npx expo start
```
Then press:
w → run on web
Scan QR → run on real phone

### For Hardware:

#### Components Required
Android phone
Internet connection
Location Access

#### Circuit Setup
Not applicable — this is a pure software mobile application.

---

## Project Documentation

### For Software:

#### Screenshots (Add at least 3)

<img width="1900" height="862" alt="image 1" src="https://github.com/user-attachments/assets/8d3d187d-5aab-4f9c-a45c-5e809ce93d7f" />
Caption: Main screen showing SOS button and Start Tracking button. This is the core interface used during emergencies.

<img width="758" height="1600" alt="image 2" src="https://github.com/user-attachments/assets/1c634d09-f9a9-445d-a1a9-5a73fae96a5f" />
Caption: Screen where users add and manage emergency contact numbers stored locally in the device.

<img width="785" height="1600" alt="image 3" src="https://github.com/user-attachments/assets/d949fc73-57c5-4d9a-8afa-245acd5b4182" />
Caption: Alert confirmation displayed when SOS is triggered, indicating message is being sent to saved contacts.

#### Diagrams

**System Architecture:**
<img width="794" height="944" alt="System_Architecture_Emergency_App" src="https://github.com/user-attachments/assets/364eeeeb-8138-4578-87c1-86ee4a6e09db" />

Explanation:

The system follows a client-side architecture:
  User interacts with React Native UI
  SOS button triggers logic handler
  App retrieves contacts from AsyncStorage
  GPS location fetched via expo-location
  SMS sent through expo-sms API
  Background tracking handled by expo-task-manager

Data Flow:
  User → UI Button → Logic Handler → Location API → SMS API → Emergency Contact
  
**Application Workflow:**

+--------+
|  User  |
+--------+
     |
     v
+----------------+
|  UI Button     |
| (Emergency Tap)|
+----------------+
     |
     v
+----------------+
|  Logic Handler |
| (App Brain)    |
+----------------+
     |
     v
+----------------+
|  Location API  |
| (Get GPS Data) |
+----------------+
     |
     v
+----------------+
|    SMS API     |
| (Send Alert)   |
+----------------+
     |
     v
+---------------------+
|  Emergency Contact  |
| (Receives Message)  |
+---------------------+
Workflow Explanation:

  User opens app
  Saves emergency contacts
  Presses SOS button or enables tracking
  App fetches live GPS location
  App sends SMS with coordinates
  Contact receives alert with map link

---

### For Hardware:
(This project is software-based and does not require physical hardware components.)
#### Schematic & Circuit

Not applicable — no circuit used.

![Schematic](Add your schematic diagram here)
*Add caption explaining the schematic*

#### Build Photos

<img width="1460" height="993" alt="TeamPhoto" src="https://github.com/user-attachments/assets/71ced016-5533-4e3e-bf3a-8ee81040588d" />

Components:
  No physical components used.
  Software stack components:
  React Native
  Expo SDK
  AsyncStorage
  Location API
  SMS API

Build:

  Build process is software compilation and packaging using:
  Node.js runtime
  Expo bundler
  Android SDK

Final Product:
  Final output is a working mobile safety application that runs on Android devices and allows emergency SOS alerts and background location tracking.

---

## Additional Documentation

### For Mobile Apps:

#### App Flow Diagram

![App Flow](docs/app-flow.png)
User Flow Explanation:

  User opens app
  User saves emergency contacts
  User chooses action:
  Press SOS button → sends emergency SMS with live location
  Press Start Tracking → enables background location monitorin
  App fetches GPS coordinates
  App sends location link to saved contacts
  Emergency contact receives alert message

The workflow is designed to minimize steps during panic situations, ensuring fast emergency communication.

#### Installation Guide

**For Android (APK):**
1. Download the APK from [Release Link]
2. Enable "Install from Unknown Sources" in your device settings:
   - Go to Settings > Security
   - Enable "Unknown Sources"
3. Open the downloaded APK file
4. Follow the installation prompts
5. Open the app and enjoy!

**For iOS (IPA) - TestFlight:**
1. Download TestFlight from the App Store
2. Open this TestFlight link: [Your TestFlight Link]
3. Click "Install" or "Accept"
4. Wait for the app to install
5. Open the app from your home screen

**Building from Source:**
```bash
# For Android
flutter build apk
# or
./gradlew assembleDebug

# For iOS
flutter build ios
# or
xcodebuild -workspace App.xcworkspace -scheme App -configuration Debug
```

---

## Project Demo

### Video
[Add your demo video link here - YouTube, Google Drive, etc.]

*Explain what the video demonstrates - key features, user flow, technical highlights*

### Additional Demos
[Add any extra demo materials/links - Live site, APK download, online demo, etc.]

---

## AI Tools Used (Optional - For Transparency Bonus)


**Tool Used:** [e.g., Gemini, ChatGPT, Claude]

**Purpose:** [What you used it for]
- Example: "Generated boilerplate React components"
- Example: "Debugging assistance for async functions"
- Example: "Code review and optimization suggestions"

**Key Prompts Used:**
- "Create a REST API endpoint for user authentication"
- "Debug this async function that's causing race conditions"
- "Optimize this database query for better performance"

**Percentage of AI-generated code:** [Approximately X%]

**Human Contributions:**
- Architecture design and planning
- Custom business logic implementation
- Integration and testing
- UI/UX design decisions

*Note: Proper documentation of AI usage demonstrates transparency and earns bonus points in evaluation!*

---

## Team Contributions

- [Name 1]: [Specific contributions - e.g., Frontend development, API integration, etc.]
- [Name 2]: [Specific contributions - e.g., Backend development, Database design, etc.]
- [Name 3]: [Specific contributions - e.g., UI/UX design, Testing, Documentation, etc.]

---

## License

This project is licensed under the [LICENSE_NAME] License - see the [LICENSE](LICENSE) file for details.

**Common License Options:**
- MIT License (Permissive, widely used)
- Apache 2.0 (Permissive with patent grant)
- GPL v3 (Copyleft, requires derivative works to be open source)

---

Made with ❤️ at TinkerHub
