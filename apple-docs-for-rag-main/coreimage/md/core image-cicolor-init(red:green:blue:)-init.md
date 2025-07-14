

- Core Image
- CIColor
-  init(red:green:blue:) 

Initializer

# init(red:green:blue:)

Creates a color object using the specified RGB color component values

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
convenience init(
    red r: CGFloat,
    green g: CGFloat,
    blue b: CGFloat
)
```

## Parameters 

`r`  

The value of the red component.

`g`  

The value of the green component.

`b`  

The value of the blue component.

## Return Value

A Core Image color object that represents an RGB color in the color space specified by the Quartz 2D constant kCGColorSpaceGenericRGB.

## See Also

### Creating Color Objects

init(string: String)

Creates a color object using the RGBA color component values specified by a string.

### Related Documentation

+ colorWithCGColor:

Creates a color object from a Quartz color.

+ colorWithRed:green:blue:alpha:

Creates a color object using the specified RGBA color component values.

