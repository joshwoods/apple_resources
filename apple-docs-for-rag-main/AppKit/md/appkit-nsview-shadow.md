

- AppKit
- NSView
-  shadow 

Instance Property

# shadow

The shadow displayed underneath the view.

macOS 10.5+

``` source
@NSCopying @MainActor
var shadow: NSShadow? { get set }
```

## Return Value

An instance of `NSShadow` that is created using the shadowColor,shadowOffset, shadowOpacity, and shadowRadius properties of the view’s layer.

## Discussion

The default value of this property is normally `nil`. When you configure any of the shadow-related properties on the view’s layer, such as the shadowColor,shadowOffset, shadowOpacity or shadowRadius properties, this property contains the NSShadow object that encapsulates that information. Assigning a new shadow object to this property sets the corresponding shadow-related properties on the view’s layer.

If the view does not have a layer, setting the value of this property has no effect.

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

var contentFilters: [CIFilter]

An array of Core Image filters to apply to the contents of the view and its sublayers.

