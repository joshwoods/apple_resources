

- SwiftUI
- VisualEffect
-  hueRotation(\_:) 

Instance Method

# hueRotation(\_:)

Applies a hue rotation effect to the view.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func hueRotation(_ angle: Angle) -> some VisualEffect
```

## Parameters 

`angle`  

The hue rotation angle to apply to the colors in the view.

## Return Value

An effect that shifts all of the colors in the view.

## Discussion

Use hue rotation effect to shift all of the colors in a view according to the angle you specify.

## See Also

### Adjusting Color

func brightness(Double) -> some VisualEffect

Brightens the view by the specified amount.

func colorEffect(Shader, isEnabled: Bool) -> some VisualEffect

Returns a new visual effect that applies `shader` to `self` as a filter effect on the color of each pixel.

func contrast(Double) -> some VisualEffect

Sets the contrast and separation between similar colors in the view.

func grayscale(Double) -> some VisualEffect

Adds a grayscale effect to the view.

func saturation(Double) -> some VisualEffect

Adjusts the color saturation of the view.

func opacity(Double) -> some VisualEffect

Sets the transparency of the view.

