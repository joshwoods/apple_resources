

- RealityKit
- RealityView
-  transformEffect(\_:) 

Instance Method

# transformEffect(\_:)

Applies an affine transformation to this view’s rendered output.

RealityKitSwiftUIiOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
nonisolated
func transformEffect(_ transform: CGAffineTransform) -> some View
```

## Parameters 

`transform`  

A CGAffineTransform to apply to the view.

## Discussion

Use `transformEffect(_:)` to rotate, scale, translate, or skew the output of the view according to the provided CGAffineTransform.

In the example below, the text is rotated at -30˚ on the `y` axis.

```
let transform = CGAffineTransform(rotationAngle: -30 * (.pi / 180))

Text("Projection effect using transforms")
    .transformEffect(transform)
    .border(Color.gray)
```

