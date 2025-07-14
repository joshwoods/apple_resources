

- UIKit
- NSTextViewportLayoutController
-  relocateViewport(to:) 

Instance Method

# relocateViewport(to:)

Relocates the viewport to the location you specify.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
func relocateViewport(to textLocation: any NSTextLocation) -> CGFloat
```

## Parameters 

`textLocation`  

An `NSTextLocation`.

## See Also

### Accessing the viewport characteristics

var viewportBounds: CGRect

Returns the visible bounds of the view, plus the overdraw area.

var viewportRange: NSTextRange?

Returns the text range of the current viewport layout.

func adjustViewport(byVerticalOffset: CGFloat)

Adjusts the viewport rect by the specified offset if needed.

func layoutViewport()

Performs layout in the viewport.

