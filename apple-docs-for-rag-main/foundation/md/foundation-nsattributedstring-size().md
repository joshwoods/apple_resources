

- Foundation
- NSAttributedString
-  size() 

Instance Method

# size()

Returns the size necessary to draw the string.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func size() -> CGSize
```

## Return Value

The minimum size required to draw the entire contents of the string.

## Discussion

You can use this method prior to drawing to compute how much space is required to draw the string.

This method may return fractional sizes. When setting the size of your view, use the ceil function to round fractional values up to the nearest whole number.

## See Also

### Related Documentation

func draw(at: CGPoint)

Draws the attributed string starting at the specified point in the current graphics context.

func draw(in: CGRect)

Draws the attributed string inside the specified bounding rectangle in the current graphics context.

### Getting metrics for the string

func boundingRect(with: CGSize, options: NSStringDrawingOptions, context: NSStringDrawingContext?) -> CGRect

Returns the bounding rectangle necessary to draw the string.

func containsAttachments(in: NSRange) -> Bool

Returns a Boolean value that indicates if the attributed string contains an attachment in the specified range.

