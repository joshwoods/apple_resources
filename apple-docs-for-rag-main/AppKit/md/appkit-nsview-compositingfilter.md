

- AppKit
- NSView
-  compositingFilter 

Instance Property

# compositingFilter

The Core Image filter used to composite the view’s contents with its background.

macOS 10.5+

``` source
@MainActor
var compositingFilter: CIFilter? { get set }
```

## Discussion

This property contains the compositing filter stored in the compositingFilter property of the view’s layer. If the view does not have a layer, setting the value of this property has no effect.

The default value of this property is `nil`, which causes content to be rendered without any special compositing effects.

## See Also

### Managing Layer-Related Properties

var alphaValue: CGFloat

The opacity of the view.

var frameCenterRotation: CGFloat

The rotation angle of the view around the center of its layer.

var backgroundFilters: [CIFilter]

An array of Core Image filters to apply to the view’s background.

var contentFilters: [CIFilter]

An array of Core Image filters to apply to the contents of the view and its sublayers.

var shadow: NSShadow?

The shadow displayed underneath the view.

