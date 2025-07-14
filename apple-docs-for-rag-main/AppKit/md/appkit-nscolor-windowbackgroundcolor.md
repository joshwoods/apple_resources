

- AppKit
- NSColor
-  windowBackgroundColor 

Type Property

# windowBackgroundColor

The color to use for the window background.

macOS

``` source
class var windowBackgroundColor: NSColor { get }
```

## Return Value

The window background color.

## Discussion

When applied to an NSBox object, this color supports Desktop Tinting in Dark Mode. With Desktop Tinting, the system modifies this color dynamically by incorporating some of the color from the underlying desktop image. The system does not apply this dynamic tinting effect to other types of views.

## See Also

### Window Colors

class var windowFrameTextColor: NSColor

The color to use for text in a window’s frame.

class var underPageBackgroundColor: NSColor

The color to use in the area beneath your window’s views.

