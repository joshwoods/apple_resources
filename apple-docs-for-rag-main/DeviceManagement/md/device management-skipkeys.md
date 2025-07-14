

- Device Management
-  SkipKeys 

Object

# SkipKeys

The list of setup panes.

iOS 7.0+iPadOS 7.0+macOS 10.9+tvOS 10.2+Device Assignment ServicesVPP License Management

``` source
object SkipKeys
```

## Properties

`Accessibility`

`string`

The key to skip the Accessibility pane. This key is not available in macOS.

`ActionButton`

`string`

The key to skip the Action Button configuration pane. This key is available in iOS 17 and later.

`Android`

`string`

If the Restore pane isn’t skipped, this is the key to remove the Move from Android option in the Restore pane on iOS. This key is available in iOS 9 and later.

`Appearance`

`string`

The key to skip the Choose Your Look screen. This key is available in iOS 13+ and macOS 10.14 and later.

`AppleID`

`string`

The key to skip Apple ID setup. This key is available in iOS 7.0+, tvOS 10.2 and later, and macOS 10.9 and later.

`AppStore`

`string`

The key to skip the App Store pane. This key is available in iOS 14.3 and later, and macOS 11.1 and later.

`Biometric`

`string`

The key to skip biometric setup. This key is available in iOS 8.1 and later, and macOS 10.12.4 and later.

`CameraButton`

`string`

The key to skip the Camera Button pane. This key is available in iOS 18 and later.

`DeviceToDeviceMigration`

`string`

The key to skip Device to Device Migration pane. This key is available in iOS 13 and later.

`Diagnostics`

`string`

The key to skip the App Analytics pane. This key is available in iOS 7 and later, tvOS 10.2 and later, and macOS 10.9 and later.

`DisplayTone`

`string`

Deprecated 

The key to skip DisplayTone setup. This key is available in iOS 9.3.2 and later, and macOS 10.13.6 and later, and deprecated in iOS 15 and macOS 12.

`EnableLockdownMode`

`string`

The key to skip the Lockdown Mode pane if an Apple ID is set up. Available in iOS 17.1 and later, and macOS 14 and later.

`FileVault`

`string`

The key to disable the FileVault Setup Assistant screen in macOS. This key is available in macOS 10.10 and later.

`HomeButtonSensitivity`

`string`

Deprecated 

The key to skip the Meet the New Home Button screen on iPhone 7, iPhone 7 Plus, iPhone 8, iPhone 8 Plus, and iPhone SE. This key is available in iOS 10 and later, and deprecated in iOS 15.

`iCloudDiagnostics`

`string`

The key to skip the iCloud Analytics screen. This key is available in macOS 10.12.4 and later.

`iCloudStorage`

`string`

The key to skip the iCloud Documents and Desktop screen in macOS. This key is available in macOS 10.13.4 and later.

`iMessageAndFaceTime`

`string`

The key to skip the iMessage and FaceTime screen in iOS. This key is available in iOS 12 and later.

`Intelligence`

`string`

The key to skip the Intelligence pane. This key is available in iOS 18 and later and macOS 15 and later.

`Keyboard`

`string`

The key to skip the Keyboard pane. This pane isn’t always skippable because it appears before the device retrieves the Cloud Configuration from the server. This key is available in iOS 13 and later.

`Location`

`string`

The key to disable Location Services. This key is available in iOS 7 and later, and macOS 10.11 and later.

`MessagingActivationUsingPhoneNumber`

`string`

The key to skip the iMessage pane. This key is available in iOS 10 and later.

`OnBoarding`

`string`

Deprecated 

The key to skip the on-boarding informational screens for user education (Go Home, Cover Sheet, Multitasking & Control Center, for example) in iOS. This key is available in iOS 11 and later, and deprecated in iOS 14.

`Passcode`

`string`

The key to hide and disable the passcode pane. This key is available in iOS 7 and later.

`Payment`

`string`

The key to skip Apple Pay setup. This key is available in iOS 8.1 and later, and macOS 10.12.4 and later.

`Privacy`

`string`

The key to skip the privacy pane. This key is available in iOS 11.13 and later, tvOS 11.13 and later, and macOS 10.13.4 and later.

`Restore`

`string`

The key to disable restoring from backup. This key is available in iOS 7 and later, and macOS 10.9 and later.

`RestoreCompleted`

`string`

The key to skip the Restore Completed pane. This key is available in iOS 14 and later.

`Safety`

`string`

The key to skip the Safety pane. This key is available in iOS 16 and later.

`ScreenSaver`

`string`

The key to skip the tvOS screen about using aerial screensavers in ATV. This key is available in tvOS 10.2 and later.

`ScreenTime`

`string`

The key to skip the Screen Time pane. This key is available in iOS 12 and later, and macOS 10.15 and later.

`SIMSetup`

`string`

The key to skip the add cellular plan pane. Skipping this pane prevents automatic eSIM setup during Setup Assistant. This key is available in iOS 12 and later.

`Siri`

`string`

The key to disable Siri. This key is available in iOS 7 and later, tvOS 10.2 and later, and macOS 10.12 and later.

`SoftwareUpdate`

`string`

The key to skip the mandatory software update screen in iOS. This key is available in iOS 12 and later.

`SpokenLanguage`

`string`

The key to skip the Dictation pane. This pane isn’t always skippable because it appears before the device retrieves the Cloud Configuration from the server. This key is available in iOS 13 and later.

`TapToSetup`

`string`

The key to skip the Tap To Set Up option in AppleTV related to using an iOS device to set up your AppleTV. This key is available in tvOS 10.2 and later.

`TermsOfAddress`

`string`

The key to skip the Terms of Address pane. This key isn’t always skippable because this pane appears before the device retrieves the Cloud Configuration from the server. This key is available in iOS 16 and later, and macOS 13 and later.

`TOS`

`string`

The key to skip Terms and Conditions. This key is available in iOS 7 and later, tvOS 10.2 and later, and macOS 10.9 and later.

`TVHomeScreenSync`

`string`

The key to skip TV home screen layout sync screen. This key is available in tvOS 11 and later.

`TVProviderSignIn`

`string`

The key to skip the TV provider sign in screen. This key is available in tvOS 11 and later.

`TVRoom`

`string`

The key to skip the “Where is this Apple TV?” screen in tvOS. This key is available in tvOS 11.4 and later.

`UpdateCompleted`

`string`

The key to skip the Software Update Complete pane. This key is available in iOS 14 and later.

`Wallpaper`

`string`

The key to skip Wallpaper setup.

This key is available in macOS 14.1 and later,

`WatchMigration`

`string`

The key to skip the screen for watch migration. This key is available in iOS 11 and later.

`WebContentFiltering`

`string`

`Welcome`

`string`

The key to skip the Get Started pane. This key is available in iOS 13 and later and macOS 15 and later.

`Zoom`

`string`

Deprecated 

The key to skip zoom setup. This key is available in iOS 8.3 and later, and deprecated in iOS 17.

`SafetyAndHandling`

`string`

