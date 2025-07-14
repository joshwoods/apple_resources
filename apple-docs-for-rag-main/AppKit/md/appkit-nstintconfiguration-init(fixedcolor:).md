

- AppKit
- NSTintConfiguration
-  init(fixedColor:) 

Initializer

# init(fixedColor:)

Creates a new tint configuration using a specific color value.

macOS 11.0+

``` source
convenience init(fixedColor color: NSColor)
```

## Parameters 

`color`  

The color used regardless of the system accent color.

## See Also

### Initializing a Tint Configuration

convenience init(preferredColor: NSColor)

Creates a new tint configuration for the system to use when the app’s preferred accent color is in use.

