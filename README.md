# Problem Solve Lab - Group A

## Overview

Problem Solve Lab is a Flutter application designed to assist users with various queries related to a specific school. The app uses a chat interface to interact with users and provide relevant information based on predefined data.

## Features

- **Chat Interface**: Users can interact with a chatbot to get answers to their queries.
- **Responsive Layout**: The app adapts to different screen sizes, providing an optimal user experience on both mobile and desktop devices.
- **Firebase Integration**: The app uses Firebase for backend services.
- **Localization**: The app supports multiple languages.

## Project Structure

- **lib/core**: Contains core functionalities and constants used throughout the app.
- **lib/feature**: Contains the main features of the app, including authentication and chat functionalities.
- **lib/main.dart**: The entry point of the application.

## Setup Instructions

1. **Clone the Repository**:
    ```sh
    git clone https://github.com/AAldossary260/problem-solve-lab.git
    cd problem-solve-lab
    ```

2. **Install Dependencies**:
    ```sh
    flutter pub get
    ```

3. **Configure Firebase**:
    - Ensure you have the `google-services.json` file for Android and `GoogleService-Info.plist` for iOS in the appropriate directories.
    - Update the `firebase_options.dart` file with your Firebase project configurations.

4. **Run the App**:
    ```sh
    flutter run
    ```

## Database Integration

The app uses Firebase as its backend service. Here’s how the database is integrated:

1. **Firebase Setup**:
    - Create a Firebase project in the Firebase Console.
    - Add your app to the Firebase project and download the `google-services.json` (for Android) and `GoogleService-Info.plist` (for iOS).
    - Place these files in the appropriate directories in your Flutter project.

2. **Firebase Configuration**:
    - The `firebase_options.dart` file contains the Firebase configuration for different platforms.
    - Initialize Firebase in the `main.dart` file using the `DefaultFirebaseOptions.currentPlatform` configuration.

3. **Data Handling**:
    - The app uses Firebase Firestore to store and retrieve chat data.
    - Firestore collections and documents are used to manage chat sessions and user data.

## Display Logic

The app uses a responsive layout to adapt to different screen sizes. Here’s how the display logic is implemented:

1. **Responsive Layout**:
    - The `ResponsaveLayout` class in `lib/core/class/responsave_layout.dart` handles the layout logic.
    - It checks the screen width and displays either the mobile or desktop layout accordingly.

2. **Chat Interface**:
    - The `ChatScreen` and `ChatWidget` classes in `lib/test.dart` manage the chat interface.
    - The chat messages are displayed using a `ListView` that dynamically updates as new messages are sent or received.

3. **Theming**:
    - The app uses a custom theme defined in `lib/main.dart`.
    - The theme includes color schemes and text styles that are applied throughout the app.

## Key Files and Their Purpose

- **lib/core/constant/links_app.dart**: Contains external links used in the app.
- **lib/core/constant/image_assets.dart**: Manages image asset paths.
- **lib/core/constant/app_routes.dart**: Defines the routes used in the app.
- **lib/core/constant/api_key.dart**: Stores the API key for the generative model.
- **lib/core/class/responsave_layout.dart**: Handles responsive layout logic.
- **lib/core/class/bg_screen.dart**: Manages background screen layout.
- **lib/main.dart**: The main entry point of the app.

