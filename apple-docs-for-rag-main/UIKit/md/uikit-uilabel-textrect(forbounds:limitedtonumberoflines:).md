

- UIKit
- UILabel
-  textRect(forBounds:limitedToNumberOfLines:) 

Instance Method

# textRect(forBounds:limitedToNumberOfLines:)

Returns the drawing rectangle for the label’s text.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func textRect(
    forBounds bounds: CGRect,
    limitedToNumberOfLines numberOfLines: Int
) -> CGRect
```

## Parameters 

`bounds`  

The bounding rectangle of the label.

`numberOfLines`  

The maximum number of lines to use for the label. The value `0` indicates the label has no maximum number of lines and the rectangle should encompass all of the text.

## Return Value

The computed drawing rectangle for the label’s text.

## Discussion

Override this method in subclasses that require changes in the label’s bounding rectangle to occur before the system performs other text layout calculations. Use the value in the `numberOfLines` parameter to limit the height of the returned rectangle to the specified number of lines of text.

The system may call this method if there was a prior call to the sizeToFit() or sizeThatFits(_:) method. Note that labels in UITableViewCell objects have sizes based on cell dimensions, and not on a requested size.

## See Also

### Drawing and positioning overrides

func drawText(in: CGRect)

Draws the label’s text, or its shadow, in the specified rectangle.

