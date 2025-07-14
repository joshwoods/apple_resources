

- AppKit
- NSView
-  contentFilters 

Instance Property

# contentFilters

An array of Core Image filters to apply to the contents of the view and its sublayers.

macOS 10.5+

``` source
@MainActor
var contentFilters: [CIFilter] { get set }
```

## Discussion

This property contains an array of CIFilter objects. This array represents the filters stored in the filters property of the view’s layer. If the view does not have a layer, setting the value of this property has no effect.

The default value of this property is an empty array.

## See Also

### Managing Layer-Related Properties

var alphaValue: CGFloat

The opacity of the view.

var frameCenterRotation: CGFloat

The rotation angle of the view around the center of its layer.

var backgroundFilters: [CIFilter]

An array of Core Image filters to apply to the view’s background.

var compositingFilter: CIFilter?

The Core Image filter used to composite the view’s contents with its background.

var shadow: NSShadow?

The shadow displayed underneath the view.

