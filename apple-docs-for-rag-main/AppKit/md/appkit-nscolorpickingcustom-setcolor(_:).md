

- AppKit
- NSColorPickingCustom
-  setColor(\_:) 

Instance Method

# setColor(\_:)

Adjusts the receiver to make the specified color the currently selected color.

macOS

``` source
@MainActor
func setColor(_ newColor: NSColor)
```

**Required**

## Parameters 

`newColor`  

The color to set as the currently selected color.

## Discussion

This method is invoked on the current color picker each time `NSColorPanel`‘s color method is invoked. If `color` is actually different from the color picker’s color (as it would be if, for example, the user dragged a color into `NSColorPanel`‘s color well), this method could be used to update the color picker’s color to reflect the change.

## See Also

### Related Documentation

Color Programming Topics

