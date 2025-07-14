

- UIKit
- UIPrintInteractionControllerDelegate
-  printInteractionController(\_:cutLengthFor:) 

Instance Method

# printInteractionController(\_:cutLengthFor:)

Asks the delegate for a length to use when cutting the page.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func printInteractionController(
    _ printInteractionController: UIPrintInteractionController,
    cutLengthFor paper: UIPrintPaper
) -> CGFloat
```

## Parameters 

`printInteractionController`  

The shared instance of UIPrintInteractionController that is managing the print job.

`paper`  

A UIPrintPaper that specifies the maximum physical and printable areas of the page.

## Return Value

The physical length of the page in points.

## Discussion

Some printers can cut a roll of print paper at a particular length. If you implement this method in your delegate, then it may be called during a print job. Your delegate should determine the length in which the content fits and return this value. When printed, the paper will be cut to this length.

## See Also

### Choosing a Paper Size for the Print Job

func printInteractionController(UIPrintInteractionController, choosePaper: [UIPrintPaper]) -> UIPrintPaper

Asks the delegate for an object that encapsulates the paper size and printing area for the print job.

func printInteractionController(UIPrintInteractionController, chooseCutterBehavior: [Any]) -> UIPrinter.CutterBehavior

Asks the delegate for the cutter behavior for the print job.

