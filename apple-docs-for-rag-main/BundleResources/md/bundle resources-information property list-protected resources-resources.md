

- Bundle Resources
- Information Property List
-  Protected resources 

API Collection

# Protected resources

Control an app’s access to protected system services and user data.

## Overview

Before your app can access certain protected resources, like the Bluetooth interface, location information, or the user’s photos, the system asks the user for permission on behalf of your app. To signal that your app needs the access, you add a `UsageDescription` key to your app’s Information Property List. You set the value associated with the key to a string that explains why your app needs access. The system displays this string when prompting the user, as described in Requesting access to protected resources.

## Topics

### Essentials

Requesting access to protected resources

Provide a purpose string that explains to a person why you need access to protected resources on their device.

Inspecting app activity data

Verify that your app accesses only the user data and network resources that you expect it to access.

### Bluetooth

NSBluetoothAlwaysUsageDescription

A message that tells the user why the app needs access to Bluetooth.

**Name:** Privacy - Bluetooth Always Usage Description

NSBluetoothPeripheralUsageDescription

A message that tells the user why the app is requesting the ability to connect to Bluetooth peripherals.

**Name:** Privacy - Bluetooth Peripheral Usage Description

Deprecated

### Calendar and reminders

NSCalendarsFullAccessUsageDescription

A message that tells people why the app is requesting access to read and write their calendar data.

**Name:** Privacy - Calendars Full Access Usage Description

NSCalendarsWriteOnlyAccessUsageDescription

A message that tells people why the app is requesting access to create calendar events.

**Name:** Privacy - Calendars Write Only Usage Description

NSRemindersFullAccessUsageDescription

A message that tells people why the app is requesting access to read and write their reminders data.

**Name:** Privacy - Reminders Full Access Usage Description

Accessing the event store

Request access to a person’s calendar data through the event store.

### Camera and microphone

Requesting authorization to capture and save media

Prompt the user to authorize access to the camera, microphone, and photo library.

Requesting Authorization for Media Capture on macOS

Prompt the user to authorize access to the camera and microphone.

NSCameraUsageDescription

A message that tells the user why the app is requesting access to the device’s camera.

**Name:** Privacy - Camera Usage Description

NSMicrophoneUsageDescription

A message that tells the user why the app is requesting access to the device’s microphone.

**Name:** Privacy - Microphone Usage Description

### Contacts

Accessing the contact store

Request permission from the person to read and write their contact data.

NSContactsUsageDescription

A message that tells the user why the app is requesting access to the user’s contacts.

**Name:** Privacy - Contacts Usage Description

### Face ID

Logging a User into Your App with Face ID or Touch ID

Supplement your own authentication scheme with biometric authentication, making it easy for users to access sensitive parts of your app.

NSFaceIDUsageDescription

A message that tells the user why the app is requesting the ability to authenticate with Face ID.

**Name:** Privacy - Face ID Usage Description

### Files and folders

NSDesktopFolderUsageDescription

A message that tells the user why the app needs access to the user’s Desktop folder.

**Name:** Privacy - Desktop Folder Usage Description

NSDocumentsFolderUsageDescription

A message that tells the user why the app needs access to the user’s Documents folder.

**Name:** Privacy - Documents Folder Usage Description

NSDownloadsFolderUsageDescription

A message that tells the user why the app needs access to the user’s Downloads folder.

**Name:** Privacy - Downloads Folder Usage Description

NSNetworkVolumesUsageDescription

A message that tells the user why the app needs access to files on a network volume.

**Name:** Privacy - Network Volumes Usage Description

NSRemovableVolumesUsageDescription

A message that tells the user why the app needs access to files on a removable volume.

**Name:** Privacy - Removable Volumes Usage Description

NSFileProviderDomainUsageDescription

A message that tells the user why the app needs access to files managed by a file provider.

**Name:** Privacy - Access to a File Provider Domain Usage Description

### Game center

NSGKFriendListUsageDescription

A message that tells the user why the app needs access to their Game Center friends list.

### Health

Setting up HealthKit

Set up and configure your HealthKit store.

NSHealthClinicalHealthRecordsShareUsageDescription

A message to the user that explains why the app requested permission to read clinical records.

**Name:** Privacy - Health Records Usage Description

NSHealthShareUsageDescription

A message to the user that explains why the app requested permission to read samples from the HealthKit store.

**Name:** Privacy - Health Share Usage Description

NSHealthUpdateUsageDescription

A message to the user that explains why the app requested permission to save samples to the HealthKit store.

**Name:** Privacy - Health Update Usage Description

NSHealthRequiredReadAuthorizationTypeIdentifiers

The clinical record data types that your app must get permission to read.

### Home

Enabling HomeKit in your app

Declare your app’s intention to use HomeKit, and get permission from the user to access home automation accessories.

NSHomeKitUsageDescription

A message that tells the user why the app is requesting access to the user’s HomeKit configuration data.

**Name:** Privacy - HomeKit Usage Description

### Location

Choosing the Location Services Authorization to Request

Determine the authorization your app needs to access location data.

NSLocationAlwaysAndWhenInUseUsageDescription

A message that tells the user why the app is requesting access to the user’s location information at all times.

**Name:** Privacy - Location Always and When In Use Usage Description

NSLocationUsageDescription

A message that tells the user why the app is requesting access to the user’s location information.

**Name:** Privacy - Location Usage Description

NSLocationWhenInUseUsageDescription

A message that tells the user why the app is requesting access to the user’s location information while the app is running in the foreground.

**Name:** Privacy - Location When In Use Usage Description

NSLocationTemporaryUsageDescriptionDictionary

A collection of messages that explain why the app is requesting temporary access to the user’s location.

**Name:** Privacy - Location Temporary Usage Description Dictionary

NSLocationAlwaysUsageDescription

A message that tells the user why the app is requesting access to the user’s location at all times.

**Name:** Privacy - Location Always Usage Description

Deprecated

NSWidgetWantsLocation

A Boolean value that indicates a widget uses the user’s location information.

**Name:** Widget wants location

NSLocationDefaultAccuracyReduced

A Boolean value that indicates whether the app requests reduced location accuracy by default.

**Name:** Privacy - Location Default Accuracy Reduced

### MediaPlayer

Requesting Access to Apple Music Library

Prompt the customer to authorize access to Apple Music library.

NSAppleMusicUsageDescription

A message that tells the user why the app is requesting access to the user’s media library.

**Name:** Privacy - Media Library Usage Description

### Motion

NSMotionUsageDescription

A message that tells the user why the app is requesting access to the device’s motion data.

**Name:** Privacy - Motion Usage Description

NSFallDetectionUsageDescription

A message to the user that explains the app’s request for permission to access fall detection event data.

**Name:** Fall Detection Usage Description

### Networking

NSLocalNetworkUsageDescription

A message that tells the user why the app is requesting access to the local network.

**Name:** Privacy - Local Network Usage Description

NSNearbyInteractionUsageDescription

A request for user permission to begin an interaction session with nearby devices.

**Name:** Privacy - Nearby Interaction Usage Description

NSNearbyInteractionAllowOnceUsageDescription

A one-time request for user permission to begin an interaction session with nearby devices.

**Name:** Privacy - Nearby Interaction Allow Once Usage Description

Deprecated

### NFC

NFCReaderUsageDescription

A message that tells the user why the app is requesting access to the device’s NFC hardware.

**Name:** Privacy - NFC Scan Usage Description

### Photos

Delivering an Enhanced Privacy Experience in Your Photos App

Adopt the latest privacy enhancements to deliver advanced user-privacy controls.

NSPhotoLibraryAddUsageDescription

A message that tells the user why the app is requesting add-only access to the user’s photo library.

**Name:** Privacy - Photo Library Additions Usage Description

NSPhotoLibraryUsageDescription

A message that tells the user why the app is requesting access to the user’s photo library.

**Name:** Privacy - Photo Library Usage Description

### Scripting

NSAppleScriptEnabled

A Boolean value indicating whether AppleScript is enabled.

**Name:** Scriptable

### Security

NSUpdateSecurityPolicy

A dictionary that identifies which apps or installer packages the operating system allows to write to the app’s bundle.

NSAppDataUsageDescription

A message that tells the user why the app needs to access files in other apps’ sandbox containers.

**Name:** Privacy - Other Application Data Usage Description

NSUserTrackingUsageDescription

A message that informs the user why an app is requesting permission to use data for tracking the user or the device.

**Name:** Privacy - Tracking Usage Description

NSAppleEventsUsageDescription

A message that tells the user why the app is requesting the ability to send Apple events.

**Name:** Privacy - AppleEvents Sending Usage Description

NSSystemAdministrationUsageDescription

A message in macOS that tells the user why the app is requesting to manipulate the system configuration.

**Name:** Privacy - System Administration Usage Description

ITSAppUsesNonExemptEncryption

A Boolean value indicating whether the app uses encryption.

**Name:** App Uses Non-Exempt Encryption

ITSEncryptionExportComplianceCode

The export compliance code provided by App Store Connect for apps that require it.

**Name:** App Encryption Export Compliance Code

### Sensors

NSSensorKitUsageDescription

A short description of the purpose of your app’s research study.

NSSensorKitUsageDetail

A dictionary that includes keys for the specific information your app collects.

NSSensorKitPrivacyPolicyURL

A hyperlink to a webpage that displays the privacy policy for your app’s research study.

### Siri

Requesting Authorization to Use Siri

Request permission from the user for Siri and Maps to communicate with your app or Intents app extension.

NSSiriUsageDescription

A message that tells the user why the app is requesting to send user data to Siri.

**Name:** Privacy - Siri Usage Description

### Speech

Asking Permission to Use Speech Recognition

Ask the user’s permission to perform speech recognition using Apple’s servers.

NSSpeechRecognitionUsageDescription

A message that tells the user why the app is requesting to send user data to Apple’s speech recognition servers.

**Name:** Privacy - Speech Recognition Usage Description

### TV

NSVideoSubscriberAccountUsageDescription

A message that tells the user why the app is requesting access to the user’s TV provider account.

**Name:** Privacy - Video Subscriber Account Usage Description

### Vision

NSWorldSensingUsageDescription

A message that tells the user why the app is requesting access to image tracking, plane detection, or scene reconstruction.

NSHandsTrackingUsageDescription

A message that tells the user why the app is requesting access to track the user’s hand position and location.

### Wallet

NSFinancialDataUsageDescription

A message that tells the user why the app is requesting access to financial data stored in Wallet.

NSIdentityUsageDescription

A message that tells the user why the app is requesting identity information.

**Name:** Privacy - Identity Usage Description

### Wi-Fi

UIRequiresPersistentWiFi

A Boolean value that indicates whether the app requires a Wi-Fi connection.

**Name:** Application uses Wi-Fi

### Deprecated keys

NSCalendarsUsageDescription

A message that tells people why the app is requesting access to their calendar data.

**Name:** Privacy - Calendars Usage Description

Deprecated

NSRemindersUsageDescription

A message that tells people why the app is requesting access to their reminders.

**Name:** Privacy - Reminders Usage Description

Deprecated

## See Also

### Services

Data and storage

Regulate documents, URLs, and other kinds of data movement and storage.

App services

Configure services provided by the app, like support for giving directions or using game controllers.

Kernel and drivers

Configure device drivers provided by the app.

