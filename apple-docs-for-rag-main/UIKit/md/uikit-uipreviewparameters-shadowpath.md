

- UIKit
- UIPreviewParameters
-  shadowPath 

Instance Property

# shadowPath

The path to use for drawing the preview’s shadow.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
@NSCopying @MainActor
var shadowPath: UIBezierPath? { get set }
```

## Discussion

If `nil`, the system uses the visiblePath to draw the shadow.

## See Also

### Configuring the preview attributes

var backgroundColor: UIColor!

The background color to display behind the preview.

var visiblePath: UIBezierPath?

The portion of the view to show in the preview.

