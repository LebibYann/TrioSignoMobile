# 👐 TrioSigno - Mobile

![TypeScript](https://img.shields.io/badge/TypeScript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white)
![ReactNative](https://img.shields.io/badge/ReactNative-%2361DAFB.svg?style=for-the-badge&logo=react&logoColor=black)
![Expo](https://img.shields.io/badge/Expo-%231C2024.svg?style=for-the-badge&logo=expo&logoColor=white)
![NativeWind](https://img.shields.io/badge/NativeWind-%2306B6D4.svg?style=for-the-badge&logo=tailwindcss&logoColor=white)

**TrioSigno** is an interactive platform dedicated to learning French Sign Language (LSF). With a modern and accessible interface, we offer a fun experience, supported by artificial intelligence, to help users learn LSF in an engaging way.


TrioSigno was our Epitech final-year project (EIP). This repository is the mobile app; the other parts live in the [EIP-TEK89](https://github.com/EIP-TEK89) organization:

| Part | Repository |
| --- | --- |
| Web + API (fullstack) | [trio-signo-fullstack](https://github.com/EIP-TEK89/trio-signo-fullstack) |
| AI sign recognition (Python) | [trio-signo-ai](https://github.com/EIP-TEK89/trio-signo-ai) |
| Shared library | [triosignolib](https://github.com/EIP-TEK89/triosignolib) |
| Mobile app (this repo) | [trio-signo-mobile](https://github.com/EIP-TEK89/trio-signo-mobile) |

<!-- TODO: add screenshots or a GIF of the app here -->

## 👤 My contribution

I was the main developer of the mobile app (33 of 39 commits):

- Authentication flow (sign-in, sign-up, token management), password change and account deletion
- Lessons, exercises and dictionary screens, connected to the API through typed service modules
- Camera-based sign recognition in exercises and dictionary practice
- Reusable UI components (loader, image wrapper, blocks), ESLint setup and a CI lint check

## 🌟 Key Features

- **AI-based sign recognition**: Users receive real-time feedback on their gestures.
- **Gamification**: Points, levels, and leaderboards to encourage progress.
- **Multi-platform accessibility**: Available on Web and Mobile.
- **Personalized reminders**: Notifications to encourage daily practice.

## 🖥️ Technologies Used

The mobile is built with the following technologies:

- **React Native** via [Expo](https://expo.dev/)
- **TypeScript** for type-safe development
- **NativeWind** (TailwindCSS for React Native)

## ⚙️ Prerequisites

- **Node.js** v14 or higher
- **npm** or **yarn**

## 🚀 Installation


1. Clone the repository:
    ```bash
    git clone https://github.com/LebibYann/TrioSignoMobile.git
    ```
2. Navigate to the project directory:
    ```bash
    cd TrioSignoMobile
    ```
3. Install the dependencies and start Expo:
    ```bash
    npm install
    npm start
    ```
## 🔧 Environment Variables
Create a ```.env``` file in the root folder with the following variables:
```ini
EXPO_PUBLIC_API_URL=https://your-api-url.com
```
> Point it to your instance of the TrioSigno API.

## 🧪 Testing

To run unit tests:
```bash
npm test
```

## 📂 Project Structure
```bash
src/
├── app/          # Screens and navigation (expo-router)
├── assets/       # Images and on-device hand-detection models (.tflite)
├── components/   # Reusable UI components, incl. AIRecognizer
├── constants/    # Shared constants
├── context/      # Context providers (auth)
├── services/     # API client and typed services
└── types/        # Types and interfaces
```

## 👥 Contributing

The steps for contributing to the project are described in the file [CONTRIBUTING.md](https://github.com/EIP-TEK89/trio-signo-fullstack/blob/main/Contributing.md).
