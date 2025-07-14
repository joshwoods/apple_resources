

- FamilyControls
- FamilyActivityPicker
-  brightness(\_:) 

Instance Method

# brightness(\_:)

Brightens this view by the specified amount.

FamilyControlsSwiftUIiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+watchOS 6.0+

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

## See Also

### Graphical Effects

func blur(radius: CGFloat, opaque: Bool) -> some View

Applies a Gaussian blur to this view.

func opacity(Double) -> some View

Sets the transparency of this view.

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

func hueRotation(Angle) -> some View

Applies a hue rotation effect to this view.

func luminanceToAlpha() -> some View

Adds a luminance to alpha effect to this view.

func shadow(color: Color, radius: CGFloat, x: CGFloat, y: CGFloat) -> some View

Adds a shadow to this view.

