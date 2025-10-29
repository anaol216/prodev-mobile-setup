# 🚀 React Native Mobile Project Setup (Expo Framework)

This README provides a quick-start guide for setting up a new **React Native** project using the **Expo Framework**, which simplifies development and testing across iOS and Android devices.

-----

## ⚙️ Prerequisites

Ensure you have the following tools installed and accessible in your environment:

  * **Node.js LTS:** The JavaScript runtime environment.
  * **npm or Yarn:** Package managers (installed with Node.js).
  * **VS Code:** (Recommended IDE).
  * **Expo Go App:** Installed on your physical Android or iOS device for easy testing.

-----

## 🛠️ Step 1: Create the Project

Use the `create-expo-app` command to quickly scaffold a new React Native project.

1.  **Open your terminal** and navigate to the directory where you want to create your project.

2.  **Run the command** to initialize the project, using the default template which includes **Expo Router** for navigation:

    ```bash
    npx create-expo-app@latest YourAppName
    ```

    (Replace `YourAppName` with your desired project name.)

3.  **Navigate** into your new project directory:

    ```bash
    cd YourAppName
    ```

-----

## ▶️ Step 2: Run the Application

The Expo CLI will start a development server and generate a QR code for testing.

1.  **Start the Expo Development Server:**

    ```bash
    npx expo start
    ```

2.  **Test on Your Device:**

      * **The terminal will display a QR code.**
      * **iOS:** Use your phone's default **Camera App** to scan the QR code.
      * **Android:** Use the **Scan QR code** option within the **Expo Go App** to scan the code.

    The app will automatically bundle and launch on your device within the Expo Go client. Any changes you save will be reflected instantly thanks to **Fast Refresh**.

-----

## 📂 Step 3: Project Structure Overview

The default template uses **Expo Router** for file-based routing, making navigation simple and intuitive.

  * `app/`: Contains all your screens and routing logic.
      * `app/_layout.tsx`: Defines the root layout and navigation structure (e.g., Stack or Tabs).
      * `app/index.tsx`: This is your main **Home Screen** (the root screen).
  * `assets/`: Stores local assets like images, fonts, and icons.
  * `components/`: Holds reusable React Native components.
  * `package.json`: Manages project dependencies and scripts.

-----

## 🎨 Step 4: Component Basics and Styling

React Native uses specific components and an in-JS styling method that is similar to CSS but uses **JavaScript objects**.

### Core Components

| Web HTML Element | React Native Component | Purpose |
| :--- | :--- | :--- |
| `<div>` | **`<View>`** | The fundamental container, supports flexbox layout. |
| `<p>`, `<h1>` | **`<Text>`** | For displaying any text. Must wrap all string content. |
| `<img />` | **`<Image>`** | For displaying local or remote images. |
| `<button>` | **`<TouchableOpacity>`** | A component that wraps others to provide a press effect. |

### Styling

Styles are defined using the `StyleSheet.create()` method imported from `react-native`.

```javascript
import { StyleSheet } from 'react-native';

const styles = StyleSheet.create({
  container: {
    // Flexbox properties like 'flex', 'justifyContent', 'alignItems' go here
    flex: 1,
    backgroundColor: '#fff',
  },
  titleText: {
    // Text-specific properties like 'fontSize', 'color', 'fontWeight' go here
    fontSize: 24,
    color: 'blue',
  },
});
```

-----

## 💡 Next Steps

  * **Install Dependencies:** Use `npm install [package-name]` or the optimized Expo version:
    ```bash
    npx expo install [package-name]
    ```
  * **Explore Routing:** Learn how to create new screens by adding new files inside the `app/` directory (e.g., `app/profile.tsx` becomes the `/profile` route).