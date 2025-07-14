

- AppKit
- NSColor
-  init(for:) Deprecated

Initializer

# init(for:)

Returns the color object specified by the given control tint.

macOS 10.0–11.0Deprecated

``` source
init(for controlTint: NSControlTint)
```

Deprecated

NSControlTint does not describe the full range of available control accent colors. Use +\[NSColor controlAccentColor\] instead.

## Parameters 

`controlTint`  

The control tint for which to return a color object. This is one of the tint settings.

## Return Value

The `NSColor` object.

## See Also

### Related Documentation

class var currentControlTint: NSControlTint

The current system control tint color.

### Creating a System Tint Color

enum NSControlTint

Constants for specifying a cell’s tint color.

