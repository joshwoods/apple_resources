

- AppKit
- NSTintConfiguration
-  baseTintColor 

Instance Property

# baseTintColor

The color the system supplies when you create a tint configuration.

macOS 11.0+

``` source
var baseTintColor: NSColor? { get }
```

## Discussion

This property is `nil` if the tint configuration wasn’t created using an NSColor object.

## See Also

### Setting the Tint Color

class var `default`: NSTintConfiguration

The system tints the content using the system default value for its context.

class var monochrome: NSTintConfiguration

The content always displays in monochrome.

var equivalentContentTintColor: NSColor?

A color object that matches the effective content tint.

