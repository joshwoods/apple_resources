

- UIKit
- UIPrintFormatter
-  draw(in:forPageAt:) 

Instance Method

# draw(in:forPageAt:)

Draws the portion of a print formatter’s content for the specified area of the specified page.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func draw(
    in rect: CGRect,
    forPageAt pageIndex: Int
)
```

## Parameters 

`rect`  

The area in which to draw the content.

`pageIndex`  

The number of the page of content to draw.

## Discussion

This method is called by the default implementation of `drawPrintFormatter:forPageAtIndex:` of the UIPrintPageRenderer class for each print formatter associated with a page.

## See Also

### Drawing the content

func rectForPage(at: Int) -> CGRect

Returns the area that encloses a specified page of content.

