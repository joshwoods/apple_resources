

- AppKit
- NSColorWell
-  takeColorFrom(\_:) 

Instance Method

# takeColorFrom(\_:)

Changes the currently selected color to the color of the specified object.

macOS

``` source
@MainActor
func takeColorFrom(_ sender: Any?)
```

## Parameters 

`sender`  

The object from which to take the new color.

## Discussion

This method attempts to access a property or accessor method named `color`. If the object doesn’t implement a `color` accessor, this method does nothing.

## See Also

### Managing the Selected Color

var color: NSColor

The currently selected color for the color well.

var supportsAlpha: Bool

A Boolean value that determines whether the color picker supports alpha values.

