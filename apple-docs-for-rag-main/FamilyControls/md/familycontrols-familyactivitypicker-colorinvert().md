

- FamilyControls
- FamilyActivityPicker
-  colorInvert() 

Instance Method

# colorInvert()

Inverts the colors in this view.

FamilyControlsSwiftUIiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+watchOS 6.0+

``` source
nonisolated
func colorInvert() -> some View
```

## Return Value

A view that inverts its colors.

## Discussion

The `colorInvert()` modifier inverts all of the colors in a view so that each color displays as its complementary color. For example, blue converts to yellow, and white converts to black.

In the example below, two red squares each have an interior green circle. The inverted square shows the effect of the square’s colors: complimentary colors for red and green — teal and purple.

```
struct InnerCircleView: View {
    var body: some View {
        Circle()
            .fill(Color.green)
            .frame(width: 40, height: 40, alignment: .center)
    }
}

struct ColorInvert: View {
    var body: some View {
        HStack {
            Color.red.frame(width: 100, height: 100, alignment: .center)
                .overlay(InnerCircleView(), alignment: .center)
                .overlay(Text("Normal")
                             .font(.callout),
                         alignment: .bottom)
                .border(Color.gray)

            Spacer()

            Color.red.frame(width: 100, height: 100, alignment: .center)
                .overlay(InnerCircleView(), alignment: .center)
                .colorInvert()
                .overlay(Text("Inverted")
                             .font(.callout),
                         alignment: .bottom)
                .border(Color.gray)
        }
        .padding(50)
    }
}
```

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

