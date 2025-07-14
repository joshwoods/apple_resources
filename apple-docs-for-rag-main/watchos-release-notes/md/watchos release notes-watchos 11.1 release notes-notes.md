

- watchOS Release Notes
-  watchOS 11.1 Release Notes 

Article

# watchOS 11.1 Release Notes

Update your apps to use new features, and test your apps against API changes.

## Overview

The watchOS 11.1 SDK provides support to develop watchOS apps for Apple Watch devices running watchOS 11.1. The SDK comes bundled with Xcode 16.1, available from the Mac App Store. For information on the compatibility requirements for Xcode 16.1, see Xcode 16.1 Release Notes.

### StoreKit

#### Resolved Issues

- Fixed: In StoreKit Testing in Xcode, the offer identifier in the subscription renewal info might be reported incorrectly for offer codes. (133774710)

### SwiftUI

#### Resolved Issues

- Fixed: Using `if #available` in @WidgetBundleBuilder and @SceneBuilder crashes on prior OS versions due to “unknown OS version.” (136098106)

### WidgetKit

#### Resolved Issues

- Fixed: Rectangular complications and Watch-specific custom Live Activity views use the wrong font metrics, causing title2 and title3 to render much larger than intended and largeTitle to render much smaller than intended. Additionally, custom Live Activity views use the wrong default font (SF Pro instead of SF Compact). (135831317)

## See Also

### watchOS 11

watchOS 11.5 Beta Release Notes

Update your apps to use new features, and test your apps against API changes.

watchOS 11.4 Release Notes

Update your apps to use new features, and test your apps against API changes.

watchOS 11.3 Release Notes

Update your apps to use new features, and test your apps against API changes.

watchOS 11.2 Release Notes

Update your apps to use new features, and test your apps against API changes.

watchOS 11 Release Notes

Update your apps to use new features, and test your apps against API changes.

