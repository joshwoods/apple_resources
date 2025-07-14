

- UIKit
- UILabel
-  drawText(in:) 

Instance Method

# drawText(in:)

Draws the label’s text, or its shadow, in the specified rectangle.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func drawText(in rect: CGRect)
```

## Parameters 

`rect`  

The rectangle in which to draw the text.

## Discussion

Don’t call this method directly. Override this method if you want to modify the default drawing behavior for the label’s text.

By the time the system calls this method, the current graphics context is already configured with the default environment and text color for drawing. In your overridden method, you can configure the current context further and then invoke `super` to do the actual drawing, or you can do the drawing yourself. If you do render the text yourself, don’t invoke `super`.

## See Also

### Drawing and positioning overrides

func textRect(forBounds: CGRect, limitedToNumberOfLines: Int) -> CGRect

Returns the drawing rectangle for the label’s text.

