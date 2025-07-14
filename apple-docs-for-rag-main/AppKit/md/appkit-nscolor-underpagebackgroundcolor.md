

- AppKit
- NSColor
-  underPageBackgroundColor 

Type Property

# underPageBackgroundColor

The color to use in the area beneath your window’s views.

macOS 10.8+

``` source
class var underPageBackgroundColor: NSColor { get }
```

## Return Value

Use this color to fill the backdrop underneath your app’s main content.

## Discussion

When applied to an NSBox object, this color supports Desktop Tinting in Dark Mode. With Desktop Tinting, the system modifies this color dynamically by incorporating some of the color from the underlying desktop image. The system does not apply this dynamic tinting effect to other types of views.

## See Also

### Window Colors

class var windowBackgroundColor: NSColor

The color to use for the window background.

class var windowFrameTextColor: NSColor

The color to use for text in a window’s frame.

