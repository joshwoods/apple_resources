

- UIKit
- UIPrintInteractionControllerDelegate
-  printInteractionController(\_:choosePaper:) 

Instance Method

# printInteractionController(\_:choosePaper:)

Asks the delegate for an object that encapsulates the paper size and printing area for the print job.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func printInteractionController(
    _ printInteractionController: UIPrintInteractionController,
    choosePaper paperList: [UIPrintPaper]
) -> UIPrintPaper
```

## Parameters 

`printInteractionController`  

The shared instance of UIPrintInteractionController that is managing the print job.

`paperList`  

An array of UIPrintPaper objects that represent combinations of paper sizes and imageable areas supported by the selected printer.

## Return Value

A UIPrintPaper object representing both the paper size and imageable area (or printable rectangle) to use for the print job.

## Discussion

This method is intended for apps (typically document-based apps) that have a notion of distinct paper sizes. The delegate can examine the objects in `paperList` to locate the paper size and printable rectangle combination that is best suited for its needs and return the encapsulating `UIPrintPaper` object. Or it can call the bestPaper(forPageSize:withPapersFrom:) class method of the UIPrintPaper class, passing in a specific page size (typically the document size), and return the object returned by that method.

## See Also

### Related Documentation

var printPaper: UIPrintPaper?

An object that represents the paper size and printing area for the print job.

### Choosing a Paper Size for the Print Job

func printInteractionController(UIPrintInteractionController, cutLengthFor: UIPrintPaper) -> CGFloat

Asks the delegate for a length to use when cutting the page.

func printInteractionController(UIPrintInteractionController, chooseCutterBehavior: [Any]) -> UIPrinter.CutterBehavior

Asks the delegate for the cutter behavior for the print job.

