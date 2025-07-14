

- UIKit
-  UIPrintInteractionControllerDelegate 

Protocol

# UIPrintInteractionControllerDelegate

An optional set of methods that the delegate of the shared print-interaction controller implements.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
protocol UIPrintInteractionControllerDelegate : NSObjectProtocol
```

## Overview

If the application has special requirements for content sizes, it can implement printInteractionController(_:choosePaper:) to return a UIPrintPaper object encapsulating the page size and the printing area to use for a print job. If you want more control of the presentation of the printing options, the delegate can return a view controller that owns the printing-options view in an implementation of printInteractionControllerParentViewController(_:). The delegate can also implement methods that are invoked when the printing user interface is presented and when it is dismissed, and when the print job begins and ends.

## Topics

### Returning a Parent View Controller

func printInteractionControllerParentViewController(UIPrintInteractionController) -> UIViewController?

Returns a parent view controller for managing the printing-options view.

### Choosing a Paper Size for the Print Job

func printInteractionController(UIPrintInteractionController, choosePaper: [UIPrintPaper]) -> UIPrintPaper

Asks the delegate for an object that encapsulates the paper size and printing area for the print job.

func printInteractionController(UIPrintInteractionController, cutLengthFor: UIPrintPaper) -> CGFloat

Asks the delegate for a length to use when cutting the page.

func printInteractionController(UIPrintInteractionController, chooseCutterBehavior: [Any]) -> UIPrinter.CutterBehavior

Asks the delegate for the cutter behavior for the print job.

### Responding to the Presentation and Dismissal of the Printing Interface

func printInteractionControllerWillPresentPrinterOptions(UIPrintInteractionController)

Tells the delegate that the device is about to display the printing-options user interface.

func printInteractionControllerDidPresentPrinterOptions(UIPrintInteractionController)

Tells the delegate that the device has presented the printing-options user interface.

func printInteractionControllerWillDismissPrinterOptions(UIPrintInteractionController)

Tells the delegate that the device is about to dismiss the printing-options user interface.

func printInteractionControllerDidDismissPrinterOptions(UIPrintInteractionController)

Tells the delegate that the device is dismissing the printing-options user interface.

### Responding to the Start and End of a Print Job

func printInteractionControllerWillStartJob(UIPrintInteractionController)

Tells the delegate that the print job is about to start.

func printInteractionControllerDidFinishJob(UIPrintInteractionController)

Tells the delegate that the print job has ended.

### Constants

enum CutterBehavior

Constants that specify the cutter behavior of a roll-fed printer.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Assigning the delegate

var delegate: (any UIPrintInteractionControllerDelegate)?

The delegate of the print-interaction controller.

