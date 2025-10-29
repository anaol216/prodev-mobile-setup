...existing code...

# prodev-mobile-app — Expo (app-example)

A starter Expo project created with create-expo-app. The production app lives in the `app` directory; this folder (`app-example`) contains the starter/example code.

## Requirements

- Node.js 18+ (or LTS)
- npm (or yarn)
- Git
- For native builds: Android Studio (Android emulator) and/or Xcode (macOS for iOS simulator)
- Windows users: run commands in PowerShell, Command Prompt, or Windows Terminal

## Quick start

1. Install dependencies
   ```bash
   npm install
   ```

2. Start Metro / Expo Dev Tools
   ```bash
   npx expo start
   ```

3. Open the app
   - Scan the QR code with Expo Go (Android/iOS)
   - Or run on emulator:
     - Android: `npx expo run:android` (requires Android Studio/emulator)
     - iOS (macOS): `npx expo run:ios`

Common helpful commands:
- Clear cache: `npx expo start -c`
- Reset starter project (moves this example to `app-example` and creates a blank `app`):  
  ```bash
  npm run reset-project
  ```

## Available npm scripts

Scripts are defined in package.json. Typical scripts:
- `start` — start Expo dev tools
- `android` / `ios` / `web` — platform runners (if present)
- `reset-project` — reset starter into `app-example`

Run:
```bash
npm run
```
to list all configured scripts.

## Project structure (key folders)

- `app/` — your application (file-based routing)
- `app-example/` — this starter/example app
- `assets/` — images, fonts, other static assets
- `package.json` — scripts and dependencies
- `README.md` — this file

This project uses Expo Router (file-based routing). Place screens and route files under `app/`.

## Debugging & tips

- Use React Native Debugger or browser dev tools for console logs and network inspection.
- When adding native modules, install with `expo prebuild` or use development builds.
- If Metro fails or assets don’t update, try `npx expo start -c`.

## Contributing

- Edit files in `app/` to start development.
- Create branches for changes, follow existing code style, and open PRs.

## Resources

- Expo docs: https://docs.expo.dev
- Expo Router: https://expo.github.io/router
- Expo Discord: https://chat.expo.dev

## License

This project follows the license defined in the repository (check LICENSE file).
