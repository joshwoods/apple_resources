

- UIKit
- UIFontMetrics
-  scaledValue(for:) 

Instance Method

# scaledValue(for:)

Scales an arbitrary layout value based on the current Dynamic Type settings.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func scaledValue(for value: CGFloat) -> CGFloat
```

## Parameters 

`value`  

The height value that you want to scale. Specify the height of the object that contains the text (at the standard Dynamic Type size) that you want to display.

## Return Value

A layout height that is scaled appropriately to accommodate the text that you want to display.

## Discussion

Use this method to scale the height of visual elements containing text. For example, if you define a button with text that can scale based on Dynamic Type, you would use this method to obtain an appropriately scaled height for your button’s background content.

## See Also

### Scaling Layout Values

func scaledValue(for: CGFloat, compatibleWith: UITraitCollection?) -> CGFloat

Scales an arbitrary layout value based on the current Dynamic Type settings and the specified traits.

