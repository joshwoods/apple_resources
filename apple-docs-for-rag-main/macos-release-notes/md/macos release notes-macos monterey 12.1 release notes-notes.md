

- macOS Release Notes
-  macOS Monterey 12.1 Release Notes 

Article

# macOS Monterey 12.1 Release Notes

Update your apps to use new features, and test your apps against API changes.

## Overview

The macOS 12.1 SDK provides support to develop apps for Mac computers running macOS Monterey 12.1. The SDK comes bundled with Xcode 13.2, available from the Mac App Store. For information on the compatibility requirements for Xcode 13.2, see Xcode 13.2 Release Notes.

### App Store

#### New Features

- StoreKit APIs that present a refund request sheet can be tested with StoreKit Testing in Xcode. Use beginRefundRequest(in:) or beginRefundRequest(for:in:) when working with AppKit or the `refundRequestSheet(for:isPresented:onDismiss:)` view modifier when working with SwiftUI. (70794860)

### Displays

#### New Features

- You can now use graphics cards that integrate the AMD Radeon RX 6600 XT GPU. (82532062)

### iCloud Mail

#### New Features

- iCloud+ subscribers can now access and use Hide My Email directly from the Mail app. (84956894)

### Reminders

#### New Features

- Tags can now be bulk renamed and deleted. (82177979)

### SwiftUI

#### Resolved Issues

- Using alert(_:isPresented:actions:message:) and doc://com.apple.documentation/documentation/swiftui/group/confirmationdialog(\_:ispresented:titlevisibility:actions:)-1v2e0 now present. (83731075)

- Pushing a ScrollView that has a background applied while inside of a stack style NavigationView when inside a TabView is now correctly tracked by the navigationBar and tabBar. (83686857)

- List correctly respects safe area insets. (83312573)

- The unnecessary New Document button in the Open Panel has been removed from document-based viewer apps. (84931806)

## See Also

### macOS 12

macOS Monterey 12.5 Release Notes

Update your apps to use new features, and test your apps against API changes.

macOS Monterey 12.4 Release Notes

Update your apps to use new features, and test your apps against API changes.

macOS Monterey 12.3 Release Notes

Update your apps to use new features, and test your apps against API changes.

macOS Monterey 12.2 Release Notes

Update your apps to use new features, and test your apps against API changes.

macOS Monterey 12.0.1 Release Notes

Update your apps to use new features, and test your apps against API changes.

