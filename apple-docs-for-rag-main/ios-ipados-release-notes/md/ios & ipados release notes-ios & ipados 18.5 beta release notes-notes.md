

- iOS &amp; iPadOS Release Notes
-  iOS & iPadOS 18.5 Beta Release Notes 

Article

# iOS & iPadOS 18.5 Beta Release Notes

Update your apps to use new features, and test your apps against API changes.

## Overview

The iOS & iPadOS 18.5 SDK provides support to develop apps for iPhone and iPad running iOS & iPadOS 18.5 beta . The SDK comes bundled with Xcode 16.4, available from the Mac App Store. For information on the compatibility requirements for Xcode 16.4, see Xcode 16.4 Release Notes.

### Apple Vision Pro app

#### Resolved Issues

- Fixed: On iOS 18.4 beta 1, the Apple Vision Pro app launches with a black screen if downloaded from the App Store. Upgrade to iOS 15.1 beta 1 and newer, and the app will launch as expected. (146814396)

### StoreKit

#### Resolved Issues

- Fixed: Calling `isEligibleForIntroOffer(for:)` will return false if there is no user account signed in. (146119524)

### Writing Tools

#### Resolved Issues

- Fixed: Resolved an issue where the attributes in the NSAttributedString passed in `writingToolsCoordinator(_:replace:in:proposedText:reason:animationParameters:completion:)` (or its companion async form) are stripped when an `NSWritingToolsCoordinator` or `UIWritingToolsCoordinator` has `resultOptions` set to `[.plainText]`. The attributes are no longer stripped but instead use the same attributes as were included by the delegate in the `NSAttributedString` returned in `writingToolsCoordinator(_:requestsContextsFor:completion:)` (or its companion async form). (144105888)

## See Also

### iOS &amp; iPadOS 18

iOS & iPadOS 18.4 Release Notes

Update your apps to use new features, and test your apps against API changes.

iOS & iPadOS 18.3 Release Notes

Update your apps to use new features, and test your apps against API changes.

iOS & iPadOS 18.2 Release Notes

Update your apps to use new features, and test your apps against API changes.

iOS & iPadOS 18.1 Release Notes

Update your apps to use new features, and test your apps against API changes.

iOS & iPadOS 18 Release Notes

Update your apps to use new features, and test your apps against API changes.

