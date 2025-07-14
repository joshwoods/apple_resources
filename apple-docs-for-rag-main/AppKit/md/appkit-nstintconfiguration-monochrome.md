

- AppKit
- NSTintConfiguration
-  monochrome 

Type Property

# monochrome

The content always displays in monochrome.

macOS 11.0+

``` source
class var monochrome: NSTintConfiguration { get }
```

## Discussion

Content marked as monochrome remains monochrome regardless of the system accent color.

## See Also

### Setting the Tint Color

class var `default`: NSTintConfiguration

The system tints the content using the system default value for its context.

var baseTintColor: NSColor?

The color the system supplies when you create a tint configuration.

var equivalentContentTintColor: NSColor?

A color object that matches the effective content tint.

