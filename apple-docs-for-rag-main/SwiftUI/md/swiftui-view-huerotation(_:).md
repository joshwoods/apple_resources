

- SwiftUI
- View
-  hueRotation(\_:) 

Instance Method

# hueRotation(\_:)

Applies a hue rotation effect to this view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

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

func saturation(Double) -> some View

Adjusts the color saturation of this view.

func grayscale(Double) -> some View

Adds a grayscale effect to this view.

func luminanceToAlpha() -> some View

Adds a luminance to alpha effect to this view.

func materialActiveAppearance(MaterialActiveAppearance) -> some View

Sets an explicit active appearance for materials in this view.

var materialActiveAppearance: MaterialActiveAppearance

The behavior materials should use for their active state, defaulting to `automatic`.

struct MaterialActiveAppearance

The behavior for how materials appear active and inactive.

