

- SwiftUI
- View
-  saturation(\_:) 

Instance Method

# saturation(\_:)

Adjusts the color saturation of this view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

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

## See Also

### Transforming colors

func brightness(Double) -> some View

Brightens this view by the specified amount.

func contrast(Double) -> some View

Sets the contrast and separation between similar colors in this view.

func colorInvert() -> some View

Inverts the colors in this view.

func colorMultiply(Color) -> some View

Adds a color multiplication effect to this view.

func grayscale(Double) -> some View

Adds a grayscale effect to this view.

func hueRotation(Angle) -> some View

Applies a hue rotation effect to this view.

func luminanceToAlpha() -> some View

Adds a luminance to alpha effect to this view.

func materialActiveAppearance(MaterialActiveAppearance) -> some View

Sets an explicit active appearance for materials in this view.

var materialActiveAppearance: MaterialActiveAppearance

The behavior materials should use for their active state, defaulting to `automatic`.

struct MaterialActiveAppearance

The behavior for how materials appear active and inactive.

