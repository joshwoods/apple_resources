

- AppKit
- NSImage
-  NSImage.SymbolConfiguration 

Class

# NSImage.SymbolConfiguration

An object that contains the specific font, style, and weight attributes to apply to a symbol image.

macOS 11.0+

``` source
class SymbolConfiguration
```

## Overview

Symbol image configuration objects include details such as the point size, scale, text style, and weight to apply to your symbol image. The system uses these details to determine which variant of the image to use and how to scale or style the image.

```
if let image = NSImage(systemSymbolName: "multiply.circle.fill",
                       accessibilityDescription: "A multiply symbol inside a filled circle.") {

    var config = NSImage.SymbolConfiguration(textStyle: .body,
                                                     scale: .large)
    config = config.applying(.init(paletteColors: [.systemTeal, .systemGray]))
    imageView.image = image.withSymbolConfiguration(config)
}
```

NSImage.SymbolConfiguration objects are immutable after you create them. If you use the applying(_:) method on the object, the new image attributes replace any previous attributes you supplied. After creating a symbol configuration object, assign it to the symbolConfiguration property of the NSImageView object you use to display the image. If you draw the image directly, use the withSymbolConfiguration(_:) method to create a new image that contains the new attributes.

For design guidance, see Human Interface Guidelines.

## Topics

### Creating a Symbol Configuration

convenience init(pointSize: CGFloat, weight: NSFont.Weight)

Creates a symbol configuration with the specified point size and font weight.

convenience init(pointSize: CGFloat, weight: NSFont.Weight, scale: NSImage.SymbolScale)

Creates a symbol configuration with the specified point size, font weight, and symbol scale.

convenience init(textStyle: NSFont.TextStyle)

Creates a symbol configuration with the specified text style.

convenience init(textStyle: NSFont.TextStyle, scale: NSImage.SymbolScale)

Creates a symbol configuration with the specified text style and symbol scale.

convenience init(scale: NSImage.SymbolScale)

Creates a symbol configuration using the scale you specify.

struct TextStyle

Constants that specify the preferred text styles you use with fonts.

enum SymbolScale

Constants that specify which scale variant of a symbol image to use.

### Applying a Configuration

func applying(NSImage.SymbolConfiguration) -> Self

Creates a configuration object by applying the values from the configuration you specify.

### Creating a Color Configuration

convenience init(paletteColors: [NSColor])

Creates a color configuration by specifying a palette of colors.

convenience init(hierarchicalColor: NSColor)

Creates a hierarchical color configuration using the color you specify.

class func preferringMulticolor() -> Self

Creates a configuration that specifies that the symbol should prefer its multicolor variant if one exists.

### Type Methods

class func preferringHierarchical() -> Self

class func preferringMonochrome() -> Self

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Creating Symbol Images

func withSymbolConfiguration(NSImage.SymbolConfiguration) -> NSImage?

Creates a new symbol image with the specified configuration.

