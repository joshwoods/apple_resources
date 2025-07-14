

- AppKit
- NSFont
-  set() 

Instance Method

# set()

Sets this font as the font for the current graphics context.

macOS

``` source
func set()
```

## Discussion

This method sets the font for the graphics system but does not affect the higher-level settings of the Cocoa text system, which are controlled by text attributes.

## See Also

### Using a Font to Draw

func set(in: NSGraphicsContext)

Sets this font as the font for the specified graphics context.

