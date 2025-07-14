

- AppKit
- NSTextViewportLayoutController
-  layoutViewport() 

Instance Method

# layoutViewport()

Performs layout in the viewport.

macOS 12.0+

``` source
func layoutViewport()
```

## See Also

### Accessing the viewport characteristics

var viewportBounds: CGRect

Returns the visible bounds of the view, plus the overdraw area.

var viewportRange: NSTextRange?

Returns the text range of the current viewport layout.

func adjustViewport(byVerticalOffset: CGFloat)

Adjusts the viewport rect by the specified offset if needed.

func relocateViewport(to: any NSTextLocation) -> CGFloat

Relocates the viewport to the location you specify.

