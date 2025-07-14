

- RealityKit
- Model3D
-  padding(\_:) 

Instance Method

# padding(\_:)

Adds a specific padding amount to each edge of this view.

RealityKitSwiftUIiOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
nonisolated
func padding(_ length: CGFloat) -> some View
```

## Parameters 

`length`  

The amount, given in points, to pad this view on all edges.

## Return Value

A view that’s padded by the amount you specify.

## Discussion

Use this modifier to add padding all the way around a view.

```
VStack {
    Text("Text padded by 10 points on each edge.")
        .padding(10)
        .border(.gray)
    Text("Unpadded text for comparison.")
        .border(.yellow)
}
```

The order in which you apply modifiers matters. The example above applies the padding before applying the border to ensure that the border encompasses the padded region:

To independently control the amount of padding for each edge, use `View/padding(_:)-6pgqq`. To pad a select set of edges by the same amount, use `View/padding(_:_:)`.

