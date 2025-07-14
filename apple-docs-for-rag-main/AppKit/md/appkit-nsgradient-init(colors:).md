

- AppKit
- NSGradient
-  init(colors:) 

Initializer

# init(colors:)

Initializes a newly allocated gradient object with an array of colors.

macOS 10.5+

``` source
convenience init?(colors colorArray: [NSColor])
```

## Parameters 

`colorArray`  

An array of `NSColor` objects representing the colors to use to initialize the gradient. There must be at least two colors in the array. The first color is placed at location 0.0 and the last at location 1.0. If there are more than two colors, the additional colors are placed at evenly spaced intervals between the first and last colors.

## Return Value

The initialized `NSGradient` object.

## See Also

### Creating a Gradient

convenience init?(starting: NSColor, ending: NSColor)

Initializes a newly allocated gradient object with two colors.

convenience init?(colorsAndLocations: (NSColor, CGFloat)...)

Initializes a newly allocated gradient object with a comma-separated list of arguments.

init?(colors: [NSColor], atLocations: UnsafePointer&lt;CGFloat>?, colorSpace: NSColorSpace)

Initializes a newly allocated gradient object with the specified colors, color locations, and color space.

init?(coder: NSCoder)

Creates a gradient from data in an unarchiver.

