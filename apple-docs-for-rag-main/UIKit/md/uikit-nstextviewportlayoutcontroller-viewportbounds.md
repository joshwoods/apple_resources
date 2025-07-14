

- UIKit
- NSTextViewportLayoutController
-  viewportBounds 

Instance Property

# viewportBounds

Returns the visible bounds of the view, plus the overdraw area.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
var viewportBounds: CGRect { get }
```

## See Also

### Accessing the viewport characteristics

var viewportRange: NSTextRange?

Returns the text range of the current viewport layout.

func adjustViewport(byVerticalOffset: CGFloat)

Adjusts the viewport rect by the specified offset if needed.

func layoutViewport()

Performs layout in the viewport.

func relocateViewport(to: any NSTextLocation) -> CGFloat

Relocates the viewport to the location you specify.

