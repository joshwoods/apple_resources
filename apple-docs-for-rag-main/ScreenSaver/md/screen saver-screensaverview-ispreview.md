

- Screen Saver
- ScreenSaverView
-  isPreview 

Instance Property

# isPreview

A Boolean value that indicates whether the screen saver view is set to a size suitable for previewing its content.

macOS 10.0+

``` source
@MainActor
var isPreview: Bool { get }
```

## Discussion

The system sets the value of this property to true when it creates a smaller preview of your screen saver. When the value is false, your view matches the size of the screen. Use this property to adjust the content you present. For example, you might change the drawing parameters or data you display in your view.

## See Also

### Drawing the view

func draw(NSRect)

Draws the screen saver view.

