

- RealityKit
- Model3D
-  saturation(\_:) 

Instance Method

# saturation(\_:)

Adjusts the color saturation of this view.

RealityKitSwiftUIiOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
nonisolated
func saturation(_ amount: Double) -> some View
```

## Parameters 

`amount`  

The amount of saturation to apply to this view.

## Return Value

A view that adjusts the saturation of this view.

## Discussion

Use color saturation to increase or decrease the intensity of colors in a view.

The example below shows a series of red squares with their saturation increasing from 0 (gray) to 100% (fully-red) in 20% increments:

```
struct Saturation: View {
    var body: some View {
        HStack {
            ForEach(0..

See Also

`contrast(_:)`

