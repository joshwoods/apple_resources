

- UIKit
-  UITargetedDragPreview 

Class

# UITargetedDragPreview

A drag item preview used by the system during lift, drop, or cancellation animation.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class UITargetedDragPreview
```

## Topics

### Initializing a targeted drag item preview

convenience init(forURL: URL, target: UIDragPreviewTarget)

Initializes a new targeted drag item preview with a URL and a drag item preview.

convenience init(forURL: URL, title: String?, target: UIDragPreviewTarget)

Initializes a new targeted drag item preview with a URL, a title, and a drag item preview.

### Replacing the preview

func retargetedPreview(with: UIDragPreviewTarget) -> UITargetedDragPreview

Returns a new targeted drag item preview based on an existing one, but with a new geometric target.

## Relationships

### Inherits From

- UITargetedPreview

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Custom drag item previews

class UIDragPreviewParameters

A set of parameters for adjusting the appearance of a drag item preview or a targeted drag item preview.

class UIDragPreview

A graphical preview for a single drag item, used by the system after a drag has started and when no related animation is running.

class UIDragPreviewTarget

A geometric specification for the source or destination of a drag item preview, used by the system when a user drops items or cancels a drag activity.

