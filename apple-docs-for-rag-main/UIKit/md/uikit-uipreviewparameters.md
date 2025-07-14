

- UIKit
-  UIPreviewParameters 

Class

# UIPreviewParameters

Additional parameters to use when animating a preview interface.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 17.0+visionOS 1.0+

``` source
@MainActor
class UIPreviewParameters
```

## Topics

### Creating preview parameters

init()

Creates a default set of preview parameters.

convenience init(textLineRects: [NSValue])

Creates a preview parameters object with information about the text you want to preview.

### Configuring the preview attributes

var backgroundColor: UIColor!

The background color to display behind the preview.

var visiblePath: UIBezierPath?

The portion of the view to show in the preview.

var shadowPath: UIBezierPath?

The path to use for drawing the preview’s shadow.

## Relationships

### Inherits From

- NSObject

### Inherited By

- UIDragPreviewParameters

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

class UIPreviewTarget

An object that specifies the container view to use for animations.

