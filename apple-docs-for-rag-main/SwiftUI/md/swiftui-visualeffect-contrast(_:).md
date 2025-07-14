

- SwiftUI
- VisualEffect
-  contrast(\_:) 

Instance Method

# contrast(\_:)

Sets the contrast and separation between similar colors in the view.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func contrast(_ amount: Double) -> some VisualEffect
```

## Parameters 

`amount`  

The intensity of color contrast to apply. negative values invert colors in addition to applying contrast.

## Return Value

An effect that applies color contrast to the view.

## Discussion

Apply contrast to a view to increase or decrease the separation between similar colors in the view.

## See Also

### Adjusting Color

func brightness(Double) -> some VisualEffect

Brightens the view by the specified amount.

func colorEffect(Shader, isEnabled: Bool) -> some VisualEffect

Returns a new visual effect that applies `shader` to `self` as a filter effect on the color of each pixel.

func grayscale(Double) -> some VisualEffect

Adds a grayscale effect to the view.

func hueRotation(Angle) -> some VisualEffect

Applies a hue rotation effect to the view.

func saturation(Double) -> some VisualEffect

Adjusts the color saturation of the view.

func opacity(Double) -> some VisualEffect

Sets the transparency of the view.

