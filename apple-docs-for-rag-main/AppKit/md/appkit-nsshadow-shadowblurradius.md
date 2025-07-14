

- AppKit
- NSShadow
-  shadowBlurRadius 

Instance Property

# shadowBlurRadius

The blur radius of the shadow.

macOS 10.0+

``` source
var shadowBlurRadius: CGFloat { get set }
```

## Discussion

This property contains the shadow’s blur radius, as measured in the default user coordinate space. A value of `0` produces no blur, while larger values produce an increasingly large blurred shadow. This value must not be negative. The default value is `0`.

## See Also

### Managing a shadow

var shadowOffset: NSSize

The shadow’s relative position, which you specify with horizontal and vertical offset values.

var shadowColor: NSColor?

The color of the shadow.

