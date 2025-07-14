

- UIKit
- UIFocusHaloEffect
-  init(roundedRect:cornerRadius:curve:) 

Initializer

# init(roundedRect:cornerRadius:curve:)

Creates a rounded halo effect using the specified corner radius and corner curve.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
convenience init(
    roundedRect rect: CGRect,
    cornerRadius: CGFloat,
    curve: CALayerCornerCurve
)
```

## See Also

### Creating a halo effect

convenience init(rect: CGRect)

Creates a rectangular halo effect using the specified rectangle.

convenience init(path: UIBezierPath)

Creates a halo effect using the specified Bézier path.

