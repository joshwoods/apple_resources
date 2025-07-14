

- AppKit
- NSShadow
-  shadowColor 

Instance Property

# shadowColor

The color of the shadow.

macOS 10.0+

``` source
@NSCopying
var shadowColor: NSColor? { get set }
```

## Discussion

The default shadow color is black with an alpha of 1/3. If you set this property to `nil`, the shadow is not drawn. The color you specify must be convertible to an RGBA color and may contain alpha information.

## See Also

### Managing a shadow

var shadowOffset: NSSize

The shadow’s relative position, which you specify with horizontal and vertical offset values.

var shadowBlurRadius: CGFloat

The blur radius of the shadow.

