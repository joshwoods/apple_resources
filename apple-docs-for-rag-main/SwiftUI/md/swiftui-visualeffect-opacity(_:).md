

- SwiftUI
- VisualEffect
-  opacity(\_:) 

Instance Method

# opacity(\_:)

Sets the transparency of the view.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func opacity(_ opacity: Double) -> some VisualEffect
```

## Parameters 

`opacity`  

A value between 0 (fully transparent) and 1 (fully opaque).

## Return Value

An effect that sets the transparency of the view.

## Discussion

When applying the `opacity(_:)` effect to a view that has already had its opacity transformed, the effect of the underlying opacity transformation is multiplied.

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

func hueRotation(Angle) -> some VisualEffect

Applies a hue rotation effect to the view.

func saturation(Double) -> some VisualEffect

Adjusts the color saturation of the view.

