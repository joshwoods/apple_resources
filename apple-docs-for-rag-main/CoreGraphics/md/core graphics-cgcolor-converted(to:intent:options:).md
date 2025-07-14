

- Core Graphics
- CGColor
-  converted(to:intent:options:) 

Instance Method

# converted(to:intent:options:)

Creates a new color in a different color space that matches the provided color.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func converted(
    to _: CGColorSpace,
    intent: CGColorRenderingIntent,
    options: CFDictionary?
) -> CGColor?
```

### Parameters

CGColorSpaceRef  
The destination color space.

to  
The destination color space.

intent  
The mechanism to use to match the color when the color is outside the gamut of the new color space.

color  
The color to convert.

options  
A dictionary of options used to convert the color. Currently, you should pass `NULL`.

### Returns

A new color in the destination color space that matches (or closely approximates) the source color.

## Discussion

To create the new color, this method creates a `CFColorConverterRef` using the options you specified and applies it to the source color.

## See Also

### Converting Between Color Spaces

class let conversionTRCSize: CFString

