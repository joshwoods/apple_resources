

- AppKit
- NSTextViewportLayoutController
-  adjustViewport(byVerticalOffset:) 

Instance Method

# adjustViewport(byVerticalOffset:)

Adjusts the viewport rect by the specified offset if needed.

macOS 12.0+

``` source
func adjustViewport(byVerticalOffset verticalOffset: CGFloat)
```

## Parameters 

`verticalOffset`  

A `CGFloat` that represents the offset amount to apply to the viewport.

## See Also

### Accessing the viewport characteristics

var viewportBounds: CGRect

Returns the visible bounds of the view, plus the overdraw area.

var viewportRange: NSTextRange?

Returns the text range of the current viewport layout.

func layoutViewport()

Performs layout in the viewport.

func relocateViewport(to: any NSTextLocation) -> CGFloat

Relocates the viewport to the location you specify.

