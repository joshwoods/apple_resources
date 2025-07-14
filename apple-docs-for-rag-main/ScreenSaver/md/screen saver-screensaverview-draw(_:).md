

- Screen Saver
- ScreenSaverView
-  draw(\_:) 

Instance Method

# draw(\_:)

Draws the screen saver view.

macOS 10.0+

``` source
@MainActor
func draw(_ rect: NSRect)
```

## Discussion

ScreenSaverView implements draw(_:) to draw a black background. Subclasses can do their drawing here or in animateOneFrame().

## See Also

### Drawing the view

var isPreview: Bool

A Boolean value that indicates whether the screen saver view is set to a size suitable for previewing its content.

