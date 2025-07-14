

- UIKit
-  UILargeContentViewerInteraction 

Class

# UILargeContentViewerInteraction

An interaction that enables a gesture to present the large content viewer for cases when supporting the largest dynamic type sizes isn’t appropriate.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class UILargeContentViewerInteraction
```

## Overview

Don’t use the large content viewer as a replacement for proper Dynamic Type support. For example, Dynamic Type allows items in a list to grow or shrink vertically to accommodate the user’s preferred font size. Rely on the large content viewer only in situations where items must remain small due to unavoidable design constraints. For example, buttons in a tab bar remain small to leave more room for the main app content.

For more information about allowing your app’s content to adjust to varying font sizes, see Add Dynamic Type support and the Human Interface Guidelines.

## Topics

### Creating large content viewer interactions

init(delegate: (any UILargeContentViewerInteractionDelegate)?)

Creates an interaction object with the specified delegate.

### Customizing large content viewer interactions

var delegate: (any UILargeContentViewerInteractionDelegate)?

An object that can fine-tune the large content viewer interactions, especially in the presence of other gesture recognizers.

var gestureRecognizerForExclusionRelationship: UIGestureRecognizer

A gesture recognizer that you can use to set up simultaneous recognition or failure relationships with other gesture recognizers.

### Detecting the large content viewer

class var isEnabled: Bool

A Boolean value that indicates whether the large content viewer is enabled on the device.

class let enabledStatusDidChangeNotification: NSNotification.Name

A notification the system posts when it enables or disables the large content viewer.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable
- UIInteraction

## See Also

### Content viewer

protocol UILargeContentViewerInteractionDelegate

An object that customizes the behavior of the large content viewer interactions.

protocol UILargeContentViewerItem

Methods that provide details about how to display your custom content in the large content viewer.

