

- Core Image
- CIColor
-  init(string:) 

Initializer

# init(string:)

Creates a color object using the RGBA color component values specified by a string.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
convenience init(string representation: String)
```

## Parameters 

`representation`  

A string that is in one of the formats returned by the `stringRepresentation` method. For example, the string:

`@"0.5 0.7 0.3 1.0"`

indicates an RGB color whose components are 50% red, 70% green, 30% blue, and 100% opaque (alpha value of `1.0`). The string representation always has four components—red, green, blue, and alpha. The default value for the alpha component is `1.0`.

## Return Value

A Core Image color object that represents an RGB color in the color space specified by the Quartz 2D constant kCGColorSpaceGenericRGB.

## See Also

### Creating Color Objects

init(red: CGFloat, green: CGFloat, blue: CGFloat)

Creates a color object using the specified RGB color component values

### Related Documentation

+ colorWithCGColor:

Creates a color object from a Quartz color.

+ colorWithRed:green:blue:alpha:

Creates a color object using the specified RGBA color component values.

