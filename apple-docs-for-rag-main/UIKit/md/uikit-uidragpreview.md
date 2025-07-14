

- UIKit
-  UIDragPreview 

Class

# UIDragPreview

A graphical preview for a single drag item, used by the system after a drag has started and when no related animation is running.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class UIDragPreview
```

## Overview

A UIDragPreview object is a visual representation of the drag item. The preview is displayed while the user moves the item across the screen with their finger (after the lift animation completes). The preview disappears when the user lifts their finger, triggering the start of the drop or cancellation animation.

## Topics

### Initializing a drag item preview

convenience init(view: UIView)

Initializes a new drag item preview with a view, using the default appearance parameters.

init(view: UIView, parameters: UIDragPreviewParameters)

Initializes a new drag item preview with a view and with a set of appearance parameters.

convenience init(forURL: URL)

Initializes a new drag item preview with a URL.

convenience init(forURL: URL, title: String?)

Initializes a drag item preview with a URL and title.

### Getting the visual appearance parameters

var parameters: UIDragPreviewParameters

The appearance parameters associated with the drag item preview.

### Accessing the view

var view: UIView

The view associated with the drag item preview.

## Relationships

### Inherits From

- NSObject

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

### Custom drag item previews

class UIDragPreviewParameters

A set of parameters for adjusting the appearance of a drag item preview or a targeted drag item preview.

class UIDragPreviewTarget

A geometric specification for the source or destination of a drag item preview, used by the system when a user drops items or cancels a drag activity.

class UITargetedDragPreview

A drag item preview used by the system during lift, drop, or cancellation animation.

