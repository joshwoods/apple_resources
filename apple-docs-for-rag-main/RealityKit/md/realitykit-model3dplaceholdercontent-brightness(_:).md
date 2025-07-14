

- RealityKit
- Model3DPlaceholderContent
-  brightness(\_:) 

Instance Method

# brightness(\_:)

Brightens this view by the specified amount.

RealityKitSwiftUIiOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
nonisolated
func brightness(_ amount: Double) -> some View
```

## Parameters 

`amount`  

A value between 0 (no effect) and 1 (full white brightening) that represents the intensity of the brightness effect.

## Return Value

A view that brightens this view by the specified amount.

## Discussion

Use `brightness(_:)` to brighten the intensity of the colors in a view. The example below shows a series of red squares, with their brightness increasing from 0 (fully red) to 100% (white) in 20% increments.

```
struct Brightness: View {
    var body: some View {
        HStack {
            ForEach(0..

