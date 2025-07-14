

- AppKit
- NSTintConfiguration
-  init(preferredColor:) 

Initializer

# init(preferredColor:)

Creates a new tint configuration for the system to use when the app’s preferred accent color is in use.

macOS 11.0+

``` source
convenience init(preferredColor color: NSColor)
```

## Parameters 

`color`  

The color used when the system accent color is `Multicolor`.

## Discussion

Use this tint configuration for custom colors designed to match app-specific accent colors, but doesn’t look appropriate matched with a user-selected color. The tint configuation only uses the preferred color when the system accent color is `Multicolor`. If the system accent color is any other color, the tint configuration defers to the accent color.

## See Also

### Initializing a Tint Configuration

convenience init(fixedColor: NSColor)

Creates a new tint configuration using a specific color value.

