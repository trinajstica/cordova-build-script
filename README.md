# Cordova Build Script for GDevelop Android Apps (for Linux)

This is a simple build script designed for automating the process of building APK and AAB packages for Android apps exported from **GDevelop** using **Cordova**.

## Features
- Automates the process of building APK and AAB packages.
- Designed specifically for **GDevelop**-exported Android apps.
- Supports **cleaning** of build files.

## Prerequisites
Before using the script, make sure you have the following installed:

- [Cordova CLI](https://cordova.apache.org/)
- [Node.js](https://nodejs.org/)
- Android SDK and JDK set up correctly
- Environment variables for your keystore:
  - `KEYSTORE_PATH`
  - `KEYSTORE_PASSWORD`
  - `KEYSTORE_ALIAS`

## Installation

1. Clone this repository to your local machine:
    ```bash
    git clone https://github.com/trinajstica/cordova-build-script.git
    cd cordova-build-script
    ```

2. Make sure you have the required dependencies for Cordova and Android:
    ```bash
    npm install -g cordova
    ```

3. Set up your keystore environment variables:
    ```bash
    export KEYSTORE_PATH="your_keystore_path"
    export KEYSTORE_PASSWORD="your_keystore_password"
    export KEYSTORE_ALIAS="your_keystore_alias"
    ```

## Usage

The script supports three commands:

### 1. Build APK
To build an APK package, run:
```bash
./build apk
```

### 2. Build AAB

To build an AAB package, run:
```bash
./build aab
```

### 3. Clean Build Files

To clean up the build-related files (APK, AAB, platforms, node_modules, etc.), run:
```bash
./build clean
```

## Notes

Make sure your GDevelop project has been exported as an Android project before running the script.
If you don't specify a command, the script will show usage instructions.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
