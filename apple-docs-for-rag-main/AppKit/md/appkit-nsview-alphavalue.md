

- AppKit
- NSView
-  alphaValue 

Instance Property

# alphaValue

The opacity of the view.

macOS 10.5+

``` source
@MainActor
var alphaValue: CGFloat { get set }
```

## Discussion

This property contains the opacity value from the view’s layer. The acceptable range of values for this property are between `0.0` (transparent) and `1.0` (opaque). The default value of this property is `1.0`.

## See Also

### Managing Layer-Related Properties

var frameCenterRotation: CGFloat

The rotation angle of the view around the center of its layer.

var backgroundFilters: [CIFilter]

An array of Core Image filters to apply to the view’s background.

var compositingFilter: CIFilter?

The Core Image filter used to composite the view’s contents with its background.

var contentFilters: [CIFilter]

An array of Core Image filters to apply to the contents of the view and its sublayers.

var shadow: NSShadow?

The shadow displayed underneath the view.

