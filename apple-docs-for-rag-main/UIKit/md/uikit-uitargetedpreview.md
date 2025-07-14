

- UIKit
-  UITargetedPreview 

Class

# UITargetedPreview

An object describing the view to use during preview-related animations.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 17.0+visionOS 1.0+

``` source
@MainActor
class UITargetedPreview
```

## Mentioned in 

Adding Writing Tools support to a custom UIKit view

## Overview

Use a UITargetedPreview to specify the view to use during an animated transition.

## Topics

### Creating a targeted preview object

Adding context menus in your app

Provide quick access to useful actions by adding context menus to your iOS app.

init(view: UIView, parameters: UIPreviewParameters, target: UIPreviewTarget)

Creates a targeted preview with the specified view, parameters, and target container.

convenience init(view: UIView, parameters: UIPreviewParameters)

Creates a targeted preview for a view in the current window and including the specified parameters.

convenience init(view: UIView)

Creates a targeted preview for a view in the current window.

### Getting the preview attributes

var view: UIView

The view that’s the target of the animation.

var target: UIPreviewTarget

The container for the target view.

var size: CGSize

The size of the view.

var parameters: UIPreviewParameters

Additional parameters to use when configuring the animations.

### Changing the target’s container

func retargetedPreview(with: UIPreviewTarget) -> UITargetedPreview

Returns a targeted preview object with the same view and parameters, but with a different target container.

## Relationships

### Inherits From

- NSObject

### Inherited By

- UITargetedDragPreview

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

class UIPreviewTarget

An object that specifies the container view to use for animations.

class UIPreviewParameters

Additional parameters to use when animating a preview interface.

