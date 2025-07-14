

- Bundle Resources
- Information Property List
-  App services 

API Collection

# App services

Configure services provided by the app, like support for giving directions or using game controllers.

## Overview

Add keys to your app’s Information Property List file that tell the system about services that your app provides.

## Topics

### Accessibility

MusicHapticsSupported

A Boolean value that indicates to the system that your app supports the Music Haptics feature.

**Name:** Supports Music Haptics

### Accessories

NSAccessorySetupSupports

An array of strings that indicates the wireless technologies AccessorySetupKit uses when discovering and configuring accessories.

**Name:** AccessorySetupKit - Supports

NSAccessorySetupBluetoothCompanyIdentifiers

An array of strings that represent the Bluetooth company identifiers for accessories that your app configures.

**Name:** AccessorySetupKit - Bluetooth Company Identifiers

NSAccessorySetupBluetoothNames

An array of strings that represent the Bluetooth device names or substrings for accessories that your app configures.

**Name:** AccessorySetupKit - Bluetooth Names

NSAccessorySetupBluetoothServices

An array of strings that represent the hexadecimal values of Bluetooth SIG-defined services or custom services for accessories your app configures.

**Name:** AccessorySetupKit - Bluetooth Services

### Ad attributions

AdNetworkIdentifiers

An array of strings that identifies the ad networks a publisher app shows advertisements for.

AttributionCopyEndpoint

A key that defines a URL that AdAttributionKit uses to deliver copies of ad attribution postbacks.

EligibleForAdAttributionKitReengagementPostbackCopies

A Boolean value that indicates whether the developer receives copies of AdAttributionKit reengagement postbacks.

### Always On display

WKSupportsAlwaysOnDisplay

A Boolean value that determines whether the system displays the app in the Always On state.

### Authentication

ASAccountAuthenticationModificationOptOutOfSecurityPromptsOnSignIn

A Boolean value that indicates the system shouldn’t show security recommendation prompts when users sign in using the app.

ASWebAuthenticationSessionWebBrowserSupportCapabilities

A collection of keys that a browser app uses to declare its ability to handle authentication requests from other apps.

### Core spotlight

CoreSpotlightActions

A dictionary that contains details about actions available to users for Spotlight search results.

### Exposure notification

ENAPIVersion

A number that specifies the version of the API to use.

ENDeveloperRegion

A string that specifies the region that the app supports.

### External accessories

UIApplicationSupportsPrintCommand

A Boolean value that indicates whether the app supports the Command-P keyboard shortcut.

**Name:** Supports Print Command

UISupportedExternalAccessoryProtocols

The protocols that the app uses to communicate with external accessory hardware.

**Name:** Supported external accessory protocols

### Games

AVGameBypassSystemSpatialAudio

A key that ignores the system spatial-audio toggle in Control Center.

GKGameCenterBadgingDisabled

A Boolean value indicating whether GameKit can add badges to a turn-based game icon.

GKShowChallengeBanners

A Boolean value that indicates whether GameKit can display challenge banners in a game.

GCSupportedGameControllers

The types of game controller profiles that the app supports or requires.

**Name:** Supported game controller types

GCSupportsControllerUserInteraction

A Boolean value indicating whether the app supports a game controller.

**Name:** Supports Controller User Interaction

GCRequiresControllerUserInteraction

The platforms for which your app requires or you recommend a game controller.

GCSupportsMultipleMicroGamepads

A Boolean value indicating whether the physical Apple TV Remote and the Apple TV Remote app operate as separate game controllers.

### Intents

INIntentsSupported

The names of the intent classes your app handles directly.

**Name:** Intents eligible for in-app handling

INIntentsRestrictedWhileLocked

The names of the intent classes your app can’t handle when the user locks the device.

**Name:** Restricted While Locked

INIntentsRestrictedWhileProtectedDataUnavailable

The names of the intent classes your app can’t handle when the user locks the device or the system blocks access to protected data.

**Name:** Intents restricted while locked or protected data unavailable

INSupportedMediaCategories

Types of media supported by your app’s media-playing intents.

**Name:** Supported intent media categories

### Interprocess communication

XPCService

### Live Activities

NSSupportsLiveActivities

A Boolean value that indicates whether an app supports Live Activities.

**Name:** Supports Live Activities

NSSupportsLiveActivitiesFrequentUpdates

A Boolean value that indicates whether an app can update its Live Activities frequently.

### Maps

MKDirectionsApplicationSupportedModes

The modes of transportation for which the app is capable of giving directions.

**Name:** Maps routing app supported modes

### Messages

NSStickerSharingLevel

### Network

NSApplicationServices

A list of service providers and the devices that they support.

### NFC

com.apple.developer.nfc.readersession.felica.systemcodes

A list of FeliCa system codes that the app supports.

**Name:** ISO18092 system codes for NFC Tag Reader Session

com.apple.developer.nfc.readersession.iso7816.select-identifiers

A list of application identifiers that the app supports.

**Name:** ISO7816 application identifiers for NFC Tag Reader Session

### Safari services

SFSafariCorrespondingIOSAppBundleIdentifier

A string bundle ID that identifies the corresponding iOS app that contains a content blocker or Safari web extension.

**Name:** Safari - Associated iOS App Bundle Identifier

SFSafariCorrespondingIOSExtensionBundleIdentifier

A string bundle ID that identifies the corresponding content blocker extension or Safari web extension on iOS.

**Name:** Safari - Associated iOS Extension Bundle Identifier

SFSafariCorrespondingMacOSAppBundleIdentifier

A string bundle ID that identifies the corresponding macOS app that contains a content blocker or Safari web extension.

**Name:** Safari - Associated macOS App Bundle Identifier

SFSafariCorrespondingMacOSExtensionBundleIdentifier

A string bundle ID that identifies the corresponding content blocker extension or Safari web extension on macOS.

**Name:** Safari - Associated macOS Extension Bundle Identifier

### Sensors

SRResearchDataGeneration

A Boolean value that indicates whether use of an app contributes data to SensorKit while the user is enrolled in a health research study.

### Service management

SMAuthorizedClients

The Service Management clients authorized to add and remove tools.

**Name:** Clients allowed to add and remove tool

SMPrivilegedExecutables

The Service Management tools owned by the app.

**Name:** Tools owned after installation

### StoreKit

SKAdNetworkItems

An array of dictionaries containing a list of ad network IDs.

SKExternalLinkAccount

A dictionary that contains localized URLs to an external website for account creation or management.

SKExternalPurchase

A string array of country codes that indicates your app supports external purchases.

SKExternalPurchaseCustomLinkRegions

An array of country code strings that indicate the regions where your app supports custom links for external purchases.

SKExternalPurchaseLink

A dictionary that contains URLs to websites where people using your app can make external purchases for supported regions.

SKExternalPurchaseMultiLink

A dictionary that contains an array of URLs to websites where people using your app can make external purchases.

SKIncludeConsumableInAppPurchaseHistory

A Boolean value that determines whether StoreKit includes finished consumable In-App Purchases in transaction information.

### User activities

NSUserActivityTypes

The user activity types that the app supports.

## See Also

### Services

Protected resources

Control an app’s access to protected system services and user data.

Data and storage

Regulate documents, URLs, and other kinds of data movement and storage.

Kernel and drivers

Configure device drivers provided by the app.

