

- UIKit
-  UIPreviewTarget 

Class

# UIPreviewTarget

An object that specifies the container view to use for animations.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 17.0+visionOS 1.0+

``` source
@MainActor
class UIPreviewTarget
```

## Overview

Create a UIPreviewTarget object when animating views to or from a separate container view. For example, use this method to animate views to or from a different part of your app’s interface.

## Topics

### Creating a preview target object

init(container: UIView, center: CGPoint, transform: CGAffineTransform)

Creates a preview target object using the specified container view and configuration details.

convenience init(container: UIView, center: CGPoint)

Creates a preview target object using the specified container view and center point.

### Getting the target attributes

var container: UIView

The container for the view being animated.

var center: CGPoint

The point in the containing view at which to place the center of the view being animated.

var transform: CGAffineTransform

An affine transform to apply to the view being animated.

## Relationships

### Inherits From

- NSObject

### Inherited By

- UIDragPreviewTarget

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol
- Sendable

## See Also

### Contextual menus

class UIContextMenuInteraction

An interaction object that you use to display relevant actions for your content.

protocol UIContextMenuInteractionDelegate

The methods for providing the set of actions to perform on your content, and for customizing the preview of that content.

class UITargetedPreview

An object describing the view to use during preview-related animations.

class UIPreviewParameters

Additional parameters to use when animating a preview interface.

