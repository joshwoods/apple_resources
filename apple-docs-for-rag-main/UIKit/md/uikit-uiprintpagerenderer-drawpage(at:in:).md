

- UIKit
- UIPrintPageRenderer
-  drawPage(at:in:) 

Instance Method

# drawPage(at:in:)

Draws a page of content for the printer.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func drawPage(
    at pageIndex: Int,
    in printableRect: CGRect
)
```

## Parameters 

`pageIndex`  

The index of the page to draw.

`printableRect`  

The rectangle in which to draw printable content.

## Discussion

The default implementation of this method calls, in sequence, drawHeaderForPage(at:in:), drawContentForPage(at:in:), drawPrintFormatter(_:forPageAt:), and drawFooterForPage(at:in:). Override this method to draw the specified page of content for the printer.

The system configures this method for drawing to the current graphics context according to UIGraphicsGetCurrentContext().

## See Also

### Drawing a page

func drawHeaderForPage(at: Int, in: CGRect)

Draws the header of a page.

func drawContentForPage(at: Int, in: CGRect)

Draws the content of a page.

func drawPrintFormatter(UIPrintFormatter, forPageAt: Int)

Performs custom drawing in addition to the specified print formatter’s drawing for a page.

func drawFooterForPage(at: Int, in: CGRect)

Draws the footer of a page.

