

- AppKit
- NSTextViewportLayoutController
-  viewportRange 

Instance Property

# viewportRange

Returns the text range of the current viewport layout.

macOS 12.0+

``` source
var viewportRange: NSTextRange? { get }
```

## See Also

### Accessing the viewport characteristics

var viewportBounds: CGRect

Returns the visible bounds of the view, plus the overdraw area.

func adjustViewport(byVerticalOffset: CGFloat)

Adjusts the viewport rect by the specified offset if needed.

func layoutViewport()

Performs layout in the viewport.

func relocateViewport(to: any NSTextLocation) -> CGFloat

Relocates the viewport to the location you specify.

