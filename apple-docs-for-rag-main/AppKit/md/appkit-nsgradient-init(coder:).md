

- AppKit
- NSGradient
-  init(coder:) 

Initializer

# init(coder:)

Creates a gradient from data in an unarchiver.

macOS 10.5+

``` source
init?(coder: NSCoder)
```

## See Also

### Creating a Gradient

convenience init?(starting: NSColor, ending: NSColor)

Initializes a newly allocated gradient object with two colors.

convenience init?(colors: [NSColor])

Initializes a newly allocated gradient object with an array of colors.

convenience init?(colorsAndLocations: (NSColor, CGFloat)...)

Initializes a newly allocated gradient object with a comma-separated list of arguments.

init?(colors: [NSColor], atLocations: UnsafePointer&lt;CGFloat>?, colorSpace: NSColorSpace)

Initializes a newly allocated gradient object with the specified colors, color locations, and color space.

