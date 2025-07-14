

- UIKit
- NSShadow
-  shadowColor 

Instance Property

# shadowColor

The color of the shadow.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var shadowColor: Any? { get set }
```

## Discussion

The default shadow color is black with an alpha of 1/3. If you set this property to `nil`, the shadow is not drawn. The color you specify must be convertible to an RGBA color and may contain alpha information.

## See Also

### Managing a shadow

var shadowOffset: CGSize

The shadow’s relative position, which you specify with horizontal and vertical offset values.

var shadowBlurRadius: CGFloat

The blur radius of the shadow.

