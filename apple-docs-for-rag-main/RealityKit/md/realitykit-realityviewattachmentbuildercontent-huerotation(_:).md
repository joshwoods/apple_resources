

- RealityKit
- RealityViewAttachmentBuilderContent
-  hueRotation(\_:) 

Instance Method

# hueRotation(\_:)

Applies a hue rotation effect to this view.

RealityKitSwiftUIiOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
nonisolated
func hueRotation(_ angle: Angle) -> some View
```

## Parameters 

`angle`  

The hue rotation angle to apply to the colors in this view.

## Return Value

A view that applies a hue rotation effect to this view.

## Discussion

Use hue rotation effect to shift all of the colors in a view according to the angle you specify.

The example below shows a series of squares filled with a linear gradient. Each square shows the effect of a 36˚ hueRotation (a total of 180˚ across the 5 squares) on the gradient:

```
struct HueRotation: View {
    var body: some View {
        HStack {
            ForEach(0..

