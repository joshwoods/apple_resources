

- AppKit
- NSFont
-  set(in:) 

Instance Method

# set(in:)

Sets this font as the font for the specified graphics context.

macOS

``` source
func set(in graphicsContext: NSGraphicsContext)
```

## Parameters 

`graphicsContext`  

The graphics context for which the font is set.

## Discussion

This method sets the font for the graphics system but does not affect the higher-level settings of the Cocoa text system, which are controlled by text attributes.

## See Also

### Using a Font to Draw

func set()

Sets this font as the font for the current graphics context.

