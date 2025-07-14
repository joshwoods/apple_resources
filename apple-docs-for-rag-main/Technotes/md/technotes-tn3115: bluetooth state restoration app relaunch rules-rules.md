

- Technotes
-  TN3115: Bluetooth State Restoration app relaunch rules 

Article

# TN3115: Bluetooth State Restoration app relaunch rules

Learn about the conditions under which an iOS app will be relaunched by Bluetooth State Restoration.

## Overview

Bluetooth State Restoration on iOS will relaunch an app in the background for pending Core Bluetooth requests. There are, though, certain conditions where the system will **not** relaunch and restore your app regardless of pending requests.

Because of user actions, it’s possible that an app may no longer be eligible to be restored in response to a Bluetooth event. Therefore it’s important to educate the users of your app, so that they understand how their actions affect the functionality of it.

Well designed apps will be resilient under such conditions.

| App or Device State        | Will the app be relaunched? |
|----------------------------|-----------------------------|
| App suspended in memory    | (see note 1)                |
| App removed from memory    | **Yes**                     |
| App crashed                | **Yes**                     |
| App Force Quit by the user | **No**                      |
| Bluetooth power toggled    | **No** (see note 2)         |
| Airplane Mode toggled      | **Yes** (see note 3)        |
| Device restarted           | **Yes** (see note 4)        |

Notes:

1.  App will be activated without needing a relaunch.

2.  Users may toggle Bluetooth power through Settings, Control Center, or via Airplane mode.

3.  Only if Bluetooth power is not toggled with Airplane Mode. Users may configure the Airplane Mode switch to not toggle Bluetooth power.

4.  If the device requires a passcode to unlock, apps will not be relaunched until the device is unlocked for the first time after a restart.

Also, it’s important to keep in mind that your app will be relaunched and restored **if and only if** it’s waiting for a specific Bluetooth event or action (like scanning, connecting, or a subscribed notification characteristic, and for peripheral apps, actively advertising), and the corresponding Bluetooth event has occurred.

For more information on Bluetooth State Preservation and Restoration refer to State Preservation and Restoration in Core Bluetooth Programming Guide

## Revision History

- **2022-02-08** Republished as TN3115. Made clarifications to the document.

- **2017-09-08** First published as QA1962.

## See Also

### Latest

TN3182: Adding privacy tracking keys to your privacy manifest

Declare the tracking domains you use in your app or third-party SDK in a privacy manifest.

TN3183: Adding required reason API entries to your privacy manifest

Declare the APIs that can potentially fingerprint devices in your app or third-party SDK in a privacy manifest.

TN3184: Adding data collection details to your privacy manifest

Declare the data your app or third-party SDK collects in a privacy manifest.

TN3181: Debugging an invalid privacy manifest

Identify common configurations that cause unsuccessful privacy manifest validation with the App Store.

TN3180: Reverting to App Store Server Notifications V1

Migrate from version 2 to version 1 of App Store Server Notifications using the Modify an App endpoint.

TN3179: Understanding local network privacy

Learn how local network privacy affects your software.

TN3178: Checking for and resolving build UUID problems

Ensure that every Mach-O image has a UUID, and that every distinct Mach-O image has its own unique UUID.

TN3177: Understanding alternate audio track groups in movie files

Learn how alternate groups collect audio tracks, and how to choose which audio track to use in your app.

TN3111: iOS Wi-Fi API overview

Explore the various Wi-Fi APIs available on iOS and their expected use cases.

TN3176: Troubleshooting Apple Pay payment processing issues

Diagnose errors that occur when processing Apple Pay payments, identify common causes, and explore potential solutions.

TN3175: Diagnosing issues with displaying the Apple Pay button on your website

Diagnose common errors received while displaying the Apple Pay button on your website by identifying the underlying causes, and explore potential solutions.

TN3174: Diagnosing issues with the Apple Pay payment sheet on your website

Diagnose errors received while presenting the Apple Pay payment sheet on your website by identifying the underlying causes of common errors and explore their potential solutions.

TN3173: Troubleshooting issues with your Apple Pay merchant identifier configuration

Diagnose errors due to invalid Apple Pay merchant identifier configurations by identifying the underlying causes of common errors and explore their potential solutions.

TN3168: Making your App Clip available in the App Store

Learn how to configure your App Clip to prevent it from being unavailable in the App Store.

TN3124: Debugging coordinate space issues

Learn techniques to help debug any coordinate space issue.

