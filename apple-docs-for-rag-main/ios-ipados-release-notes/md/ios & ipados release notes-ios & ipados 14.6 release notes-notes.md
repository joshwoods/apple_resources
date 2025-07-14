

- iOS &amp; iPadOS Release Notes
-  iOS & iPadOS 14.6 Release Notes 

Article

# iOS & iPadOS 14.6 Release Notes

Update your apps to use new features, and test your apps against API changes.

## Overview

To develop apps for iOS & iPadOS 14.6, build your apps against the iOS 14.5 SDK or later. The SDK comes bundled with Xcode 12.5, available from the Mac App Store. For information on the compatibility requirements for Xcode 12.5, see Xcode 12.5 Release Notes.

### General

#### Resolved Issues

- Fixed an issue during startup where iPhone may experience reduced performance. (77540788)

### SKAdNetwork

#### New Features

- Devices can now send install-validation postbacks to multiple ad networks that sign their ads using SKAdNetwork version 3.0. One ad network receives a postback with a `did-win` parameter value of `true` for the ad impression that wins the ad attribution. Up to five other ad networks receive a postback with a `did-win` value of `false` if their ad impressions qualified for, but didn’t win, the attribution. (72917087)

### Software Update

#### New Features

- You can now directly update your iOS or iPadOS device to the latest Release Candidate without removing the beta profile. After updating to the Release Candidate, you can choose to update to the next available beta or uninstall the profile to remove your device from the beta program. (66256273)

### Xcode

#### Deprecations

- Don’t use the iOS MinimumOSVersion information property list key to declare the minimum release of macOS in which your app runs. Use LSMinimumSystemVersion instead. (73890473)

  - Future releases of macOS ignore the `MinimumOSVersion` key in Mac apps, including apps built with Mac Catalyst.

  - Future releases of macOS use the `LSMinimumSystemVersion` key in iOS apps built with Xcode 12.5 or later. If an iOS app doesn’t include an `LSMinimumSystemVersion` key, future releases of macOS compare the app’s `MinimumOSVersion` with the version of its Mac Catalyst runtime to determine compatibility.

## See Also

### iOS &amp; iPadOS 14

iOS & iPadOS 14.7 Release Notes

Update your apps to use new features, and test your apps against API changes.

iOS & iPadOS 14.5.1 Release Notes

Update your apps to use new features, and test your apps against API changes.

iOS & iPadOS 14.5 Release Notes

Update your apps to use new features, and test your apps against API changes.

iOS & iPadOS 14.4 Release Notes

Update your apps to use new features, and test your apps against API changes.

iOS & iPadOS 14.3 Release Notes

Update your apps to use new features, and test your apps against API changes.

iOS & iPadOS 14.2 Release Notes

Update your apps to use new features, and test your apps against API changes.

iOS & iPadOS 14 Release Notes

Update your apps to use new features, and test your apps against API changes.

