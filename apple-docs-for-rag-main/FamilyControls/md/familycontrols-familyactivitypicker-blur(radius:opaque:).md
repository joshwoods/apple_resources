

- FamilyControls
- FamilyActivityPicker
-  blur(radius:opaque:) 

Instance Method

# blur(radius:opaque:)

Applies a Gaussian blur to this view.

FamilyControlsSwiftUIiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+watchOS 6.0+

``` source
nonisolated
func blur(
    radius: CGFloat,
    opaque: Bool = false
) -> some View
```

## Parameters 

`radius`  

The radial size of the blur. A blur is more diffuse when its radius is large.

`opaque`  

A Boolean value that indicates whether the blur renderer permits transparency in the blur output. Set to `true` to create an opaque blur, or set to `false` to permit transparency.

## Discussion

Use `blur(radius:opaque:)` to apply a gaussian blur effect to the rendering of this view.

The example below shows two `Text` views, the first with no blur effects, the second with `blur(radius:opaque:)` applied with the `radius` set to `2`. The larger the radius, the more diffuse the effect.

```
struct Blur: View {
    var body: some View {
        VStack {
            Text("This is some text.")
                .padding()
            Text("This is some blurry text.")
                .blur(radius: 2.0)
        }
    }
}
```

## See Also

### Graphical Effects

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

func luminanceToAlpha() -> some View

Adds a luminance to alpha effect to this view.

func shadow(color: Color, radius: CGFloat, x: CGFloat, y: CGFloat) -> some View

Adds a shadow to this view.

