

- UIKit
- UIPrintInteractionControllerDelegate
-  printInteractionController(\_:chooseCutterBehavior:) 

Instance Method

# printInteractionController(\_:chooseCutterBehavior:)

Asks the delegate for the cutter behavior for the print job.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func printInteractionController(
    _ printInteractionController: UIPrintInteractionController,
    chooseCutterBehavior availableBehaviors: [Any]
) -> UIPrinter.CutterBehavior
```

## Parameters 

`printInteractionController`  

The shared instance of UIPrintInteractionController that is managing the print job.

`availableBehaviors`  

An array of NSNumber objects identifying the printer’s available cutter behaviors. Each number corresponds to one of the constants defined in UIPrinter.CutterBehavior.

## Return Value

The cutter behavior to use for the print job. The value must correspond to one of the constants in the `availableBehaviors` parameter.

## Discussion

Some roll-fed printers support different options for cutting the paper. If you implement this method in your delegate, then it may be called during a print job. Your delegate method should determine when to make cuts and return the appropriate value.

## See Also

### Choosing a Paper Size for the Print Job

func printInteractionController(UIPrintInteractionController, choosePaper: [UIPrintPaper]) -> UIPrintPaper

Asks the delegate for an object that encapsulates the paper size and printing area for the print job.

func printInteractionController(UIPrintInteractionController, cutLengthFor: UIPrintPaper) -> CGFloat

Asks the delegate for a length to use when cutting the page.

