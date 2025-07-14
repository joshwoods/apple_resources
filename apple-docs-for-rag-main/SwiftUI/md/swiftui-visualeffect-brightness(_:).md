

- SwiftUI
- VisualEffect
-  brightness(\_:) 

Instance Method

# brightness(\_:)

Brightens the view by the specified amount.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func brightness(_ amount: Double) -> some VisualEffect
```

## Parameters 

`amount`  

A value between 0 (no effect) and 1 (full white brightening) that represents the intensity of the brightness effect.

## Return Value

An effect that brightens the view by the specified amount.

## See Also

### Adjusting Color

func colorEffect(Shader, isEnabled: Bool) -> some VisualEffect

Returns a new visual effect that applies `shader` to `self` as a filter effect on the color of each pixel.

func contrast(Double) -> some VisualEffect

Sets the contrast and separation between similar colors in the view.

func grayscale(Double) -> some VisualEffect

Adds a grayscale effect to the view.

func hueRotation(Angle) -> some VisualEffect

Applies a hue rotation effect to the view.

func saturation(Double) -> some VisualEffect

Adjusts the color saturation of the view.

func opacity(Double) -> some VisualEffect

Sets the transparency of the view.

