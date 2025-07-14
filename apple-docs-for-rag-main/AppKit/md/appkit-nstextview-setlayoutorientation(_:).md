

- AppKit
- NSTextView
-  setLayoutOrientation(\_:) 

Instance Method

# setLayoutOrientation(\_:)

Changes the receiver’s layout orientation and invalidates the contents.

macOS 10.7+

``` source
@MainActor
func setLayoutOrientation(_ orientation: NSLayoutManager.TextLayoutOrientation)
```

## Parameters 

`orientation`  

The text layout orientation.

## Discussion

Unlike other `NSTextView` properties, this is not shared by sibling views. It also rotates the bounds 90 degrees, swaps horizontal and vertical bits of the autoresizingMask mask, and reconfigures isHorizontallyResizable and isVerticallyResizable properties accordingly. Also, if enclosingScrollView returns non-`nil`, it reconfigures the horizontal and vertical ruler views, the horizontal and vertical scrollers, and the frame.

## See Also

### Changing layout orientation

func changeLayoutOrientation(Any?)

An action method that sets the layout orientation of the text.

