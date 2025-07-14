

- UIKit
- UIPrintPageRenderer
-  drawPrintFormatter(\_:forPageAt:) 

Instance Method

# drawPrintFormatter(\_:forPageAt:)

Performs custom drawing in addition to the specified print formatter’s drawing for a page.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func drawPrintFormatter(
    _ printFormatter: UIPrintFormatter,
    forPageAt pageIndex: Int
)
```

## Parameters 

`printFormatter`  

A UIPrintFormatter object associated with the page at `pageIndex`.

`pageIndex`  

The index of the page for `printFormatter` to draw on.

## Discussion

The system invokes this method for each print formatter associated with the specified page. The default implementation invokes the draw(in:forPageAt:) method of each UIPrintFormatter object.

Override this method to intermix custom drawing with the formatter drawing — for example, by adding an overlay or underlay graphic. Call draw(in:forPageAt:) to have the print formatter draw its portion of the page.

The system configures this method for drawing to the current graphics context according to UIGraphicsGetCurrentContext().

## See Also

### Drawing a page

func drawPage(at: Int, in: CGRect)

Draws a page of content for the printer.

func drawHeaderForPage(at: Int, in: CGRect)

Draws the header of a page.

func drawContentForPage(at: Int, in: CGRect)

Draws the content of a page.

func drawFooterForPage(at: Int, in: CGRect)

Draws the footer of a page.

