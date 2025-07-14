

- UIKit
- NSTextLineFragment
-  draw(at:in:) 

Instance Method

# draw(at:in:)

Renders the line fragment contents at the rendering origin.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
func draw(
    at point: CGPoint,
    in context: CGContext
)
```

## Parameters 

`point`  

The origin as a `CGPoint`.

`context`  

The drawing context.

## Discussion

You can specify the origin as (`NSMinX(typographicBounds) + glyphOrigin.x, NSMinY(typographicBounds) + glyphOrigin.y)` relative to the line fragment group coordinate system.

