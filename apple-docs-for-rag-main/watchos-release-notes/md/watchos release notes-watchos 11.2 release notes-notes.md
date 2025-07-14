

- watchOS Release Notes
-  watchOS 11.2 Release Notes 

Article

# watchOS 11.2 Release Notes

Update your apps to use new features, and test your apps against API changes.

## Overview

The watchOS 11.2 SDK provides support to develop watchOS apps for Apple Watch devices running watchOS 11.2. The SDK comes bundled with Xcode 16.2, available from the Mac App Store. For information on the compatibility requirements for Xcode 16.2, see Xcode 16.2 Release Notes.

### Battery Health

#### Resolved Issues

- Fixed: This update addresses potential inaccurate estimates of battery health reporting for some devices on watchOS 11.2 Beta 1 & 2. (139724084)

### StoreKit

#### Resolved Issues

- Fixed: Resolved an issue where using `SubscriptionStoreView` might cause an app to crash when running watchOS 11. If your app runs on watchOS versions 11.0 or 11.1, use the ‘buttons’ subscription store control style to work around the crash. (138045666)

### SwiftUI

#### Resolved Issues

- Fixed: Compiling in the Swift 6 language mode might cause an `@Entry` error due to “static property `defaultValue` is not concurrency-safe because non-‘Sendable’ type”. (133885814)

- Fixed: Views won’t accept dropped directories if UTType.directory or UTType.fileURL are not in the list of accepted content types for drop. (138158126)

## See Also

### watchOS 11

watchOS 11.5 Beta Release Notes

Update your apps to use new features, and test your apps against API changes.

watchOS 11.4 Release Notes

Update your apps to use new features, and test your apps against API changes.

watchOS 11.3 Release Notes

Update your apps to use new features, and test your apps against API changes.

watchOS 11.1 Release Notes

Update your apps to use new features, and test your apps against API changes.

watchOS 11 Release Notes

Update your apps to use new features, and test your apps against API changes.

