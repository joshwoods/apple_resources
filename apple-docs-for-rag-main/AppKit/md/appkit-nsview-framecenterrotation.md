

- AppKit
- NSView
-  frameCenterRotation 

Instance Property

# frameCenterRotation

The rotation angle of the view around the center of its layer.

macOS 10.5+

``` source
@MainActor
var frameCenterRotation: CGFloat { get set }
```

## Discussion

This property contains the angle of rotation of the view’s frame around its center. If you changed the underlying layer’s anchorPoint property, the result of setting this property is undefined.

## See Also

### Managing Layer-Related Properties

var alphaValue: CGFloat

The opacity of the view.

var backgroundFilters: [CIFilter]

An array of Core Image filters to apply to the view’s background.

var compositingFilter: CIFilter?

The Core Image filter used to composite the view’s contents with its background.

var contentFilters: [CIFilter]

An array of Core Image filters to apply to the contents of the view and its sublayers.

var shadow: NSShadow?

The shadow displayed underneath the view.

