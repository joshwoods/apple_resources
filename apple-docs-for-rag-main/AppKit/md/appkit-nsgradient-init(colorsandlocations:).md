

- AppKit
- NSGradient
-  init(colorsAndLocations:) 

Initializer

# init(colorsAndLocations:)

Initializes a newly allocated gradient object with a comma-separated list of arguments.

macOS 10.9+

``` source
convenience init?(colorsAndLocations objects: (NSColor, CGFloat)...)
```

## See Also

### Creating a Gradient

convenience init?(starting: NSColor, ending: NSColor)

Initializes a newly allocated gradient object with two colors.

convenience init?(colors: [NSColor])

Initializes a newly allocated gradient object with an array of colors.

init?(colors: [NSColor], atLocations: UnsafePointer&lt;CGFloat>?, colorSpace: NSColorSpace)

Initializes a newly allocated gradient object with the specified colors, color locations, and color space.

init?(coder: NSCoder)

Creates a gradient from data in an unarchiver.

