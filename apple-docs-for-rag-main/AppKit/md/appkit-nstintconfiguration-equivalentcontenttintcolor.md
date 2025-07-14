

- AppKit
- NSTintConfiguration
-  equivalentContentTintColor 

Instance Property

# equivalentContentTintColor

A color object that matches the effective content tint.

macOS 11.0+

``` source
var equivalentContentTintColor: NSColor? { get }
```

## Discussion

The value of this property is an NSColor that matches the represented content tint. This property is `nil` if the system can’t represent the content tint as an NSColor.

## See Also

### Setting the Tint Color

class var `default`: NSTintConfiguration

The system tints the content using the system default value for its context.

class var monochrome: NSTintConfiguration

The content always displays in monochrome.

var baseTintColor: NSColor?

The color the system supplies when you create a tint configuration.

