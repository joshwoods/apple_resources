

- UIKit
- UIPrintPageRenderer
-  drawContentForPage(at:in:) 

Instance Method

# drawContentForPage(at:in:)

Draws the content of a page.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func drawContentForPage(
    at pageIndex: Int,
    in contentRect: CGRect
)
```

## Parameters 

`pageIndex`  

The index of the page on which to draw content.

`contentRect`  

The area in which to draw content, in the coordinate system of the printable rectangle. This area is equal to printableRect minus headerHeight and footerHeight.

## Discussion

The default implementation of this method does nothing. Override this method to draw the content of the specified page.

The system configures this method for drawing to the current graphics context according to UIGraphicsGetCurrentContext().

## See Also

### Drawing a page

func drawPage(at: Int, in: CGRect)

Draws a page of content for the printer.

func drawHeaderForPage(at: Int, in: CGRect)

Draws the header of a page.

func drawPrintFormatter(UIPrintFormatter, forPageAt: Int)

Performs custom drawing in addition to the specified print formatter’s drawing for a page.

func drawFooterForPage(at: Int, in: CGRect)

Draws the footer of a page.

