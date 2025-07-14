

- AppKit
- NSColor
-  usingType(\_:) 

Instance Method

# usingType(\_:)

Returns a version of the color object that is compatible with the specified color type.

macOS 10.13+

``` source
func usingType(_ type: NSColor.ColorType) -> NSColor?
```

## Parameters 

`type`  

The type of color object that you want. For example, if you want a color object containing RGB components, specify NSColor.ColorType.componentBased.

## Return Value

A compatible color object, or `nil` if a compatible color object is not available.

## Discussion

Before accessing the details of an NSColor object, use this method to ensure that you have an object capable of returning those details. For example, before you access the component values, make sure you have a color object of type NSColor.ColorType.componentBased. For some types of colors, conversions to a compatible color type may be possible.

## See Also

### Working with the Color Space

var type: NSColor.ColorType

The type of the color object.

enum ColorType

Constants that indicate the color’s type, and which methods may be called on the color object.

var colorSpace: NSColorSpace

The color space associated with the color.

var colorSpaceName: NSColorSpaceName

The name of the color space associated with the color.

Deprecated

struct NSColorSpaceName

Constants that specify color space names.

