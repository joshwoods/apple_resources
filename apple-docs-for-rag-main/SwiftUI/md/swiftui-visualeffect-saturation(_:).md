

- SwiftUI
- VisualEffect
-  saturation(\_:) 

Instance Method

# saturation(\_:)

Adjusts the color saturation of the view.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func saturation(_ amount: Double) -> some VisualEffect
```

## Parameters 

`amount`  

The amount of saturation to apply to the view.

## Return Value

An effect that adjusts the saturation of the view.

## Discussion

Use color saturation to increase or decrease the intensity of colors in a view.

See Also

`contrast(_:)`

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

func opacity(Double) -> some VisualEffect

Sets the transparency of the view.

