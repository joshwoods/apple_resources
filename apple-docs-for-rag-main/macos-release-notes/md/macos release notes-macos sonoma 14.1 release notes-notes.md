

- macOS Release Notes
-  macOS Sonoma 14.1 Release Notes 

Article

# macOS Sonoma 14.1 Release Notes

Update your apps to use new features, and test your apps against API changes.

## Overview

The macOS 14 SDK provides support to develop apps for Mac computers running Sonoma 14.1. The SDK comes bundled with Xcode 15, available from the Mac App Store. For information on the compatibility requirements for Xcode 15, see Xcode 15 Release Notes.

### Remote Widgets

#### Resolved Issues

- Fixed: Remote Widgets might render blank on mismatched iOS and macOS releases. (115436466)

### Wallet

#### Resolved Issues

- Fixed: Some event ticket passes might fail to ingest into Wallet when added from a website on a Mac. (115216417)

### WidgetKit

#### Known Issues

- In widgets `Text(_:style:)` doesn’t animate its content by default. (107582710)

  **Workaround:** To explicitly request an animation, use the `View.contentTransition(_:)` modifier.

### iPhone 12 in France

#### Notes

- Updates the iPhone 12 for users in France to accommodate a test protocol for Specific Absorption Rate (SAR) testing. For more information, visit this website: https://support.apple.com/kb/HT213923 (116601274)

## See Also

### macOS 14

macOS Sonoma 14.6 Release Notes

Update your apps to use new features, and test your apps against API changes.

macOS Sonoma 14.5 Release Notes

Update your apps to use new features, and test your apps against API changes.

macOS Sonoma 14.4 Release Notes

Update your apps to use new features, and test your apps against API changes.

macOS Sonoma 14.3 Release Notes

Update your apps to use new features, and test your apps against API changes.

macOS Sonoma 14.2 Release Notes

Update your apps to use new features, and test your apps against API changes.

macOS Sonoma 14 Release Notes

Update your apps to use new features, and test your apps against API changes.

