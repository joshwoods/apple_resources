

- AppKit
- NSGradient
-  init(starting:ending:) 

Initializer

# init(starting:ending:)

Initializes a newly allocated gradient object with two colors.

macOS 10.5+

``` source
convenience init?(
    starting startingColor: NSColor,
    ending endingColor: NSColor
)
```

## Parameters 

`startingColor`  

The starting color of the gradient. The location of this color is fixed at 0.0.

`endingColor`  

The ending color of the gradient. The location of this color is fixed at 1.0.

## Return Value

The initialized `NSGradient` object.

## See Also

### Related Documentation

Cocoa Drawing Guide

### Creating a Gradient

convenience init?(colors: [NSColor])

Initializes a newly allocated gradient object with an array of colors.

convenience init?(colorsAndLocations: (NSColor, CGFloat)...)

Initializes a newly allocated gradient object with a comma-separated list of arguments.

init?(colors: [NSColor], atLocations: UnsafePointer&lt;CGFloat>?, colorSpace: NSColorSpace)

Initializes a newly allocated gradient object with the specified colors, color locations, and color space.

init?(coder: NSCoder)

Creates a gradient from data in an unarchiver.

