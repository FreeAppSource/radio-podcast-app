# Radio Podcast App

> 👨‍💻 Developed by **[Suresh Kumar Meesala](https://github.com/SureshKumarMeesala)** · 🎨 UI design by **Lucid.studio** (credits below)

A mobile app built with **React Native (0.88+)**, **Expo SDK 58+** and **Expo Router**, using **JavaScript and JSX (`.js`, `.jsx`)**. Every screen is built from the original Sketch design `radio-podcast-app-ui-kit-lucid-studio.sketch` by **Lucid.studio**: one route per artboard, with the artboard's layout, colours, images and text.

![Radio Podcast App screens](./showcase.jpg)

## 📱 Screens (5 design artboards)

Listed in the order of the app's flow. "Taps" is the number of tap targets wired on the screen (buttons, tabs, back arrows, list rows).

| # | Screen (artboard) | Route | Size | Taps |
|---|---|---|---|---|
| 1 | **00_splash_screen** · start screen | `src/app/s-00-splash-screen.jsx` | 414 × 896 | 1 |
| 2 | **01_channel** | `src/app/s-01-channel.jsx` | 414 × 896 | 2 |
| 3 | **02_channel** | `src/app/s-02-channel.jsx` | 414 × 896 | 2 |
| 4 | **03_channel** | `src/app/s-03-channel.jsx` | 414 × 896 | 2 |
| 5 | **04_player** | `src/app/s-04-player.jsx` | 414 × 896 | 2 |

Screenshots of every screen are in [`screenshots/`](./screenshots).

## 🧩 How it's built

- `src/screens/*.json`: each design artboard converted to screen data (vector shapes, gradients, image fills, masks, shadows, blurs and rich text, positioned as in the design), plus its tap targets
- `src/sketch/SketchScreen.jsx`: draws a screen at the device's width with `react-native-svg`, native `Text`/`TextInput` and `expo-blur`, and handles navigation between screens
- `src/app/`: Expo Router routes, one per artboard (`index.jsx` opens the start screen)
- `assets/images/`: images used by the design

## 🛠️ Tech Stack

- **Framework**: React Native 0.88+ / Expo SDK 58+
- **Navigation**: Expo Router (file-based routing)
- **Language**: JavaScript & JSX (`.js`, `.jsx`)
- **Rendering**: `react-native-svg`, `expo-blur`
- **Fonts**: Google Fonts via `@expo-google-fonts` (Inter), standing in for the design's original fonts where those aren't free

<!-- run-locally:start -->

## ▶️ Run locally

```bash
npm install
npx expo start
```

Then press `i` for the iOS simulator, `a` for Android, or `w` for the web, or scan the QR code with Expo Go.

<!-- run-locally:end -->

<!-- developer:start -->

## 👨‍💻 Developer

This React Native app was developed by **Suresh Kumar Meesala**.

| | |
|---|---|
| Developer | [Suresh Kumar Meesala](https://github.com/SureshKumarMeesala) |
| GitHub | [@SureshKumarMeesala](https://github.com/SureshKumarMeesala) |
| Organization | [FreeAppSource](https://github.com/FreeAppSource) |
| Repository | <https://github.com/FreeAppSource/radio-podcast-app> |

<!-- developer:end -->

---

<!-- design-credits:start -->

## 🎨 Design Credits

This app is based on the free **Radio Podcast App Concept** design by **Lucid.studio**, downloaded from Sketch App Sources. All visual design credit goes to the designer. The screens are reproduced from the original Sketch file; fonts that aren't free are replaced with similar Google Fonts, so some details may differ slightly from the original.

| | |
|---|---|
| Designer | [Lucid.studio](https://www.sketchappsources.com/contributor/lucid.studio) |
| Original design | [Radio Podcast App Concept](https://dribbble.com/shots/9657958-Radio-Podcast-App-UI-Kit) |
| Downloaded from | [Sketch App Sources](https://www.sketchappsources.com/free-source/4233-radio-podcast-app-ui-kit-sketch-freebie-resource.html) |
| Dribbble | <http://www.dribbble.com/LucidBerlin> |
| Original file | `radio-podcast-app-ui-kit-lucid-studio.sketch` |
| License / usage | Not stated on the page. Free download; give credit (Sketch App Sources Terms). Confirm with the designer before commercial use. The designers ask: "In case you will use it for your project, let us know and share it with us!" |

**Attribution:**

> UI design: "Radio Podcast App Concept" by Lucid.studio (https://dribbble.com/shots/9657958-Radio-Podcast-App-UI-Kit), downloaded from Sketch App Sources (https://www.sketchappsources.com/free-source/4233-radio-podcast-app-ui-kit-sketch-freebie-resource.html).

The original design source files are not included in this repository; get them from the links above. This app's **code** is released under the [MIT License](./LICENSE); the visual design remains the designer's (see [NOTICE](./NOTICE)).

Photos, brand logos and avatars inside the design may belong to third parties and are not covered by the designer's permission.

<!-- design-credits:end -->
