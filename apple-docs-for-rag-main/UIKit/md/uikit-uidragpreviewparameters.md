

- UIKit
-  UIDragPreviewParameters 

Class

# UIDragPreviewParameters

A set of parameters for adjusting the appearance of a drag item preview or a targeted drag item preview.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class UIDragPreviewParameters
```

## Overview

You can refine the appearance of a preview by providing additional parameters when creating a UIDragPreview or UITargetedDragPreview object. The parameters specify different visual aspects of the preview, including the background color and the visible area of the view associated with the preview.

## Relationships

### Inherits From

- UIPreviewParameters

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

class UIDragPreview

A graphical preview for a single drag item, used by the system after a drag has started and when no related animation is running.

class UIDragPreviewTarget

A geometric specification for the source or destination of a drag item preview, used by the system when a user drops items or cancels a drag activity.

class UITargetedDragPreview

A drag item preview used by the system during lift, drop, or cancellation animation.

