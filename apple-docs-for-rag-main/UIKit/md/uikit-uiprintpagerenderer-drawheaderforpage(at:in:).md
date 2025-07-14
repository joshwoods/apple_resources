

- UIKit
- UIPrintPageRenderer
-  drawHeaderForPage(at:in:) 

Instance Method

# drawHeaderForPage(at:in:)

Draws the header of a page.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func drawHeaderForPage(
    at pageIndex: Int,
    in headerRect: CGRect
)
```

## Parameters 

`pageIndex`  

The index of the page on which to draw the header.

`headerRect`  

The rectangle in which to draw the header content. This rectangle uses the coordinate system of the paper rectangle (paperRect), with the origin of the coordinates at the top-left corner of the sheet.

## Discussion

The default implementation of this method does nothing. The system doesn’t call this method if headerHeight isn’t a positive value. Override this method to draw the header of the specified page.

The system configures this method for drawing to the current graphics context according to UIGraphicsGetCurrentContext().

## See Also

### Drawing a page

func drawPage(at: Int, in: CGRect)

Draws a page of content for the printer.

func drawContentForPage(at: Int, in: CGRect)

Draws the content of a page.

func drawPrintFormatter(UIPrintFormatter, forPageAt: Int)

Performs custom drawing in addition to the specified print formatter’s drawing for a page.

func drawFooterForPage(at: Int, in: CGRect)

Draws the footer of a page.

