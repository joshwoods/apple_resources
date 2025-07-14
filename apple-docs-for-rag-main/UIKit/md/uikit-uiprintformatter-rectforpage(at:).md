

- UIKit
- UIPrintFormatter
-  rectForPage(at:) 

Instance Method

# rectForPage(at:)

Returns the area that encloses a specified page of content.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func rectForPage(at pageIndex: Int) -> CGRect
```

## Parameters 

`pageIndex`  

The index number of a page.

## Return Value

A rectangle enclosing the content area for page `pageIndex`.

## Discussion

Returns CGRectZero if the print formatter draws no content on the specified page.

## See Also

### Drawing the content

func draw(in: CGRect, forPageAt: Int)

Draws the portion of a print formatter’s content for the specified area of the specified page.

