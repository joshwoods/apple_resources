

- Updates
-  Bundle Resources updates 

Article

# Bundle Resources updates

Learn about important changes to Bundle Resources.

## Overview

Browse notable changes in Bundle Resources.

## June 2024

### New entitlements

- Enable access to a Personalized Sound Profile to allow the app to use the information in the profile to render audio with com.apple.developer.spatial-audio.profile-access.

- Enable access to head tracking info to allow an app to render audio with head tracking with com.apple.developer.coremotion.head-pose.

- Allow CoreMIDI to match MIDIDriverKit drivers with devices that support MIDI with com.apple.developer.driverkit.family.midi.

### Updated entitlement

- Define the app category to enable Cellular Network Slicing with 5G Network Slicing App Category. To set the application category for streaming apps, use `streaming-9001`. You can also set the category to `gaming-6014` for gaming apps, and `communication-9000` for communication apps.

### New Info.plist keys

- Indicate if the game app bypasses system spatial audio with AVGameBypassSystemSpatialAudio.

- Indicate to the system that your app receives copies of re-engagement postbacks, a type of postback introduced in iOS 17.5, with EligibleForAdAttributionKitReengagementPostbackCopies.

- Indicate to the system that your app supports the Music Haptics feature with MusicHapticsSupported.

- Indicate to the system the interfaces AccessorySetupKit uses to discover and configure accessories using Bluetooth or Wi-Fi with NSAccessorySetupSupports.

- Provide the company identifier for a Bluetooth accessory when enabling the use of AccessorySetupKit via `NSAccessorySetupKitEnabled` with NSAccessorySetupBluetoothCompanyIdentifiers.

- Provide the name for a Bluetooth accessory when enabling the use of AccessorySetupKit via `NSAccessorySetupKitEnabled` with NSAccessorySetupBluetoothNames.

- Provide the services for a Bluetooth accessory when enabling the use of AccessorySetupKit via `NSAccessorySetupKitEnabled` with NSAccessorySetupBluetoothServices.

- Provide a message that tells the user why the app requests access to financial data stored in Wallet with NSFinancialDataUsageDescription.

- Track “finished” consumable in-app purchases in StoreKit and return the transactions when iterating the `Transaction` APIs with SKIncludeConsumableInAppPurchaseHistory.

## See Also

### Technology updates

Accelerate updates

Learn about important changes to Accelerate.

Accessibility updates

Learn about important changes to Accessibility.

ActivityKit updates

Learn about important changes in ActivityKit.

AdAttributionKit Updates

Learn about important changes to AdAttributionKit.

App Intents updates

Learn about important changes in App Intents.

AppKit updates

Learn about important changes to AppKit.

Apple Intelligence updates

Learn about important changes to Apple Intelligence.

Apple Pencil updates

Learn about important changes to Apple Pencil.

ARKit updates

Learn about important changes to ARKit.

Audio Toolbox updates

Learn about important changes to Audio Toolbox.

AuthenticationServices updates

Learn about important changes to AuthenticationServices.

AVFAudio updates

Learn about important changes to AVFAudio.

AVFoundation updates

Learn about important changes to AVFoundation.

ContactsUI updates

Learn about important changes to ContactsUI.

Core Location updates

Learn about important changes to Core Location.

