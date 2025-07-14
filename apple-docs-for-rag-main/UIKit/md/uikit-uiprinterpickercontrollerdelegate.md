

- UIKit
-  UIPrinterPickerControllerDelegate 

Protocol

# UIPrinterPickerControllerDelegate

A set of methods for managing the presentation and dismissal of a printer picker interface.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
protocol UIPrinterPickerControllerDelegate : NSObjectProtocol
```

## Overview

You also use the methods of this protocol to influence the content displayed in the picker and to respond when the user selects a printer. Implement the methods of this protocol in your own custom object and assign that object to the delegate property of your UIPrinterPickerController object before presenting it. When you present the picker, it calls the methods of your delegate at appropriate times to ask for information or provide you with information about the state of the picker interface. For more information about presenting a printer picker interface, see UIPrinterPickerController.

## Topics

### Filtering the List of Printers

func printerPickerController(UIPrinterPickerController, shouldShow: UIPrinter) -> Bool

Asks the delegate if the specified printer should be included in the picker.

### Handling the Printer Selection

func printerPickerControllerDidSelectPrinter(UIPrinterPickerController)

Tells the delegate that a printer was selected.

### Responding to Printer Picker Events

func printerPickerControllerParentViewController(UIPrinterPickerController) -> UIViewController?

Asks the delegate to provide the view controller to act as the parent of the printer picker.

func printerPickerControllerWillPresent(UIPrinterPickerController)

Tells the delegate that the printer picker is about to be displayed.

func printerPickerControllerDidPresent(UIPrinterPickerController)

Tells the delegate that the printer picker was displayed and is now visible.

func printerPickerControllerWillDismiss(UIPrinterPickerController)

Tells the delegate that the printer picker is about to be dismissed.

func printerPickerControllerDidDismiss(UIPrinterPickerController)

Tells the delegate that the printer picker was dismissed.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Managing the printer picker interface

var delegate: (any UIPrinterPickerControllerDelegate)?

The delegate for the printer picker controller.

