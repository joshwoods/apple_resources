

- AppKit
- NSColor
-  withSystemEffect(\_:) 

Instance Method

# withSystemEffect(\_:)

Returns a new color object that represents the current color modified to include the specified visual effect.

macOS 10.14+

``` source
func withSystemEffect(_ systemEffect: NSColor.SystemEffect) -> NSColor
```

## Parameters 

`systemEffect`  

The visual effect you want to apply to a view or control.

## Discussion

Instead of defining separate colors for user interactions with a view, use this method to retrieve the appropriate color for use with those interactions. This method blends the current color with an appropriate modifier and returns the results. For example, specifying NSColor.SystemEffect.pressed for the `systemEffect` parameter yields the color to use when you want your view to appear as if it had been pressed. This method takes the current appearance into account, returning an appropriately modified color for both light and dark appearances.

## See Also

### Applying Specific Appearances to Colors

enum SystemEffect

Constants for user interactions that change the appearance of a view or control.

