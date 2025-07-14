

- UIKit
-  UIVisualEffectView 

Class

# UIVisualEffectView

An object that implements some complex visual effects.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UIVisualEffectView
```

## Overview

Depending on the desired effect, the effect may affect content layered behind the view or content added to the visual effect view’s contentView. Apply a visual effect view to an existing view and then apply a UIBlurEffect or UIVibrancyEffect object to apply a blur or vibrancy effect to the existing view. After you add the visual effect view to the view hierarchy, add any subviews to the contentView property of the visual effect view. Don’t add subviews directly to the visual effect view itself.

### Set the correct alpha value

When using the UIVisualEffectView class, avoid alpha values that are less than 1. Creating views that are partially transparent causes the system to combine the view and all the associated subviews during an offscreen render pass. UIVisualEffectView objects need to be combined as part of the content they’re layered on top of in order to look correct. Setting the alpha to less than 1 on the visual effect view or any of its superviews causes many effects to look incorrect or not show up at all.

### Use masks with a visual effect view

Masks directly applied to a UIVisualEffectView are forwarded to the internal views that provide the visual effect, including the contentView itself. You can also apply masks directly to the contentView. Applying a mask to a superview of a UIVisualEffectView object causes the effect to fail, and an exception is thrown.

Any mask provided to UIVisualEffectView isn’t the view that actually performs the mask. UIKit makes a copy of the view and applies it to each subview. To reflect a size change to the mask, you must apply the change to the original mask and reset it on the effect view.

### Capture a snapshot of a visual effect view

Many effects require support from the window that hosts the UIVisualEffectView. Attempting to take a snapshot of only the UIVisualEffectView results in a snapshot that doesn’t contain the effect. To take a snapshot of a view hierarchy that contains a UIVisualEffectView, you must take a snapshot of the entire UIWindow or UIScreen that contains it.

## Topics

### Creating a visual effect view

init(effect: UIVisualEffect?)

Creates a new visual effect view with the designated visual effect.

init?(coder: NSCoder)

Creates a visual effect view from data in an unarchiver.

### Retrieving view information

var contentView: UIView

A view object that can have a visual effect view added to it.

var effect: UIVisualEffect?

The visual effect provided by the view.

## Relationships

### Inherits From

- UIView

### Conforms To

- CALayerDelegate
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding
- NSTouchBarProvider
- Sendable
- UIAccessibilityIdentification
- UIActivityItemsConfigurationProviding
- UIAppearance
- UIAppearanceContainer
- UICoordinateSpace
- UIDynamicItem
- UIFocusEnvironment
- UIFocusItem
- UIFocusItemContainer
- UILargeContentViewerItem
- UIPasteConfigurationSupporting
- UIPopoverPresentationControllerSourceItem
- UIResponderStandardEditActions
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Visual effects

class UIVisualEffect

An initializer for visual effect views and blur and vibrancy effect objects.

class UIVibrancyEffect

An object that amplifies and adjusts the color of the content layered behind a visual effect view.

class UIBlurEffect

An object that applies a blurring effect to the content layered behind a visual effect view.

