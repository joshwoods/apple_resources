

- Foundation
- NSAttributedString
-  draw(at:) 

Instance Method

# draw(at:)

Draws the attributed string starting at the specified point in the current graphics context.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func draw(at point: CGPoint)
```

## Parameters 

`point`  

The point in the current graphics context where you want to start drawing the string. The coordinate system of the graphics context is usually defined by the view in which you are drawing.

## Discussion

This method draws the entire string starting at the specified point. This method draws the line using the attributes specified in the attributed string itself. If newline characters are present in the string, those characters are honored and cause subsequent text to be placed on the next line underneath the starting point.

There must be either a focused view or an active graphics context when you call this method.

## See Also

### Related Documentation

func size() -> CGSize

Returns the size necessary to draw the string.

@MainActor func lockFocus()

Locks the focus on the view, so subsequent commands take effect in the view’s window and coordinate system.

Deprecated

### Drawing the attributed string

func draw(in: CGRect)

Draws the attributed string inside the specified bounding rectangle in the current graphics context.

func draw(with: CGRect, options: NSStringDrawingOptions, context: NSStringDrawingContext?)

Draws the attributed string in the specified bounding rectangle using the provided options.

