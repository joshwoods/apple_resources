

- FamilyControls
- FamilyActivityPicker
-  luminanceToAlpha() 

Instance Method

# luminanceToAlpha()

Adds a luminance to alpha effect to this view.

FamilyControlsSwiftUIiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+watchOS 6.0+

``` source
nonisolated
func luminanceToAlpha() -> some View
```

## Return Value

A view with the luminance to alpha effect applied.

## Discussion

Use this modifier to create a semitransparent mask, with the opacity of each part of the modified view controlled by the luminance of the corresponding part of the original view. Regions of lower luminance become more transparent, while higher luminance yields greater opacity.

In particular, the modifier maps the red, green, and blue components of each input pixel’s color to a grayscale value, and that value becomes the alpha component of a black pixel in the output. This modifier produces an effect that’s equivalent to using the `feColorMatrix` filter primitive with the `luminanceToAlpha` type attribute, as defined by the Scalable Vector Graphics (SVG) 2 specification.

The example below defines a `Palette` view as a series of rectangles, each composed as a `Color` with a particular white value, and then displays two versions of the palette over a blue background:

```
struct Palette: View {
    var body: some View {
        HStack(spacing: 0) {
            ForEach(0..

The unmodified version of the palette contains rectangles that range from solid black to solid white, thus with increasing luminance. The second version of the palette, which has the `luminanceToAlpha()` modifier applied, allows the background to show through in an amount that corresponds inversely to the luminance of the input.

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

func grayscale(Double) -> some View

Adds a grayscale effect to this view.

func hueRotation(Angle) -> some View

Applies a hue rotation effect to this view.

func shadow(color: Color, radius: CGFloat, x: CGFloat, y: CGFloat) -> some View

Adds a shadow to this view.

