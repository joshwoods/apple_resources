

- UIKit
-  UIKeyboardLayoutGuide 

Class

# UIKeyboardLayoutGuide

A layout guide that represents the space the keyboard occupies in your app’s layout.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
@MainActor
class UIKeyboardLayoutGuide
```

## Overview

Configure the keyboard layout guide, and activate or deactivate constraints so your app’s layout adjusts to the keyboard in different situations. See Adjusting your layout with keyboard layout guide for an example of how to dynamically respond to keyboard presentation, dismissal, and movement.

## Topics

### Supporting floating and undocked keyboards

var followsUndockedKeyboard: Bool

A Boolean value that determines if the layout guide tracks the keyboard when it’s undocked from the bottom of the screen.

### Adjusting dismissal sensitivity

var keyboardDismissPadding: CGFloat

A value that adds padding above the keyboard to increase the size of the touch area for the scrolling dismissal gesture.

### Configuring safe area usage

var usesBottomSafeArea: Bool

A Boolean value that indicates whether the layout guide uses the view’s safe area layout guide.

## Relationships

### Inherits From

- UITrackingLayoutGuide

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- Sendable
- UIPopoverPresentationControllerSourceItem

## See Also

### Keyboard layout

Adjusting your layout with keyboard layout guide

Respond dynamically to keyboard movement by using the tracking features of the keyboard layout guide.

class UITrackingLayoutGuide

A layout guide that automatically activates and deactivates layout constraints depending on its proximity to edges.

