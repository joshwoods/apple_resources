

- SwiftUI
- HoverEffectContent
-  transformEffect(\_:) 

Instance Method

# transformEffect(\_:)

Applies an affine transformation to the view’s rendered output.

visionOS 2.0+

``` source
func transformEffect(_ transform: CGAffineTransform) -> some HoverEffectContent
```

## Parameters 

`transform`  

A CGAffineTransform to apply to the view.

## Return Value

An effect that applies an affine transformation to the view’s rendered output.

## Discussion

Use `transformEffect(_:)` to rotate, scale, translate, or skew the output of the view according to the provided CGAffineTransform.

