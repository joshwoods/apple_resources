

- AppKit
- NSGradient
-  init(colors:atLocations:colorSpace:) 

Initializer

# init(colors:atLocations:colorSpace:)

Initializes a newly allocated gradient object with the specified colors, color locations, and color space.

macOS 10.5+

``` source
init?(
    colors colorArray: [NSColor],
    atLocations locations: UnsafePointer?,
    colorSpace: NSColorSpace
)
```

## Parameters 

`colorArray`  

An array of `NSColor` objects representing the colors in the gradient.

`locations`  

An array of `CGFloat` values containing the location for each color in the gradient. Each value must be in the range 0.0 to 1.0. There must be the same number of locations as are colors in the `colorArray` parameter.

`colorSpace`  

The color space to use for the gradient.

## Return Value

The initialized `NSGradient` object.

## Discussion

This method is the designated initializer of `NSGradient`. The colors in the `colorArray` parameter are converted to the specified color space if they are not already in that color space.

Typically, at least one color should have a location of 0.0 and one should have a location of 1.0. If these locations are not specified, the color at the closest color stop is used to fill the gap.

## See Also

### Creating a Gradient

convenience init?(starting: NSColor, ending: NSColor)

Initializes a newly allocated gradient object with two colors.

convenience init?(colors: [NSColor])

Initializes a newly allocated gradient object with an array of colors.

convenience init?(colorsAndLocations: (NSColor, CGFloat)...)

Initializes a newly allocated gradient object with a comma-separated list of arguments.

init?(coder: NSCoder)

Creates a gradient from data in an unarchiver.

