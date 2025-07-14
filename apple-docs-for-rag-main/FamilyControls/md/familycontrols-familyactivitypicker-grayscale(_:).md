

- FamilyControls
- FamilyActivityPicker
-  grayscale(\_:) 

Instance Method

# grayscale(\_:)

Adds a grayscale effect to this view.

FamilyControlsSwiftUIiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+watchOS 6.0+

``` source
nonisolated
func grayscale(_ amount: Double) -> some View
```

## Parameters 

`amount`  

The intensity of grayscale to apply from 0.0 to less than 1.0. Values closer to 0.0 are more colorful, and values closer to 1.0 are less colorful.

## Return Value

A view that adds a grayscale effect to this view.

## Discussion

A grayscale effect reduces the intensity of colors in this view.

The example below shows a series of red squares with their grayscale effect increasing from 0 (reddest) to 99% (fully desaturated) in approximate 20% increments:

```
struct Saturation: View {
    var body: some View {
        HStack {
            ForEach(0..

## See Also

### Graphical Effects

func blur(radius: CGFloat, opaque: Bool) -> some View

Applies a Gaussian blur to this view.

func opacity(Double) -> some View

Sets the transparency of this view.

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

func hueRotation(Angle) -> some View

Applies a hue rotation effect to this view.

func luminanceToAlpha() -> some View

Adds a luminance to alpha effect to this view.

func shadow(color: Color, radius: CGFloat, x: CGFloat, y: CGFloat) -> some View

Adds a shadow to this view.

