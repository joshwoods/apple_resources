

- UIKit
- UIPrinterPickerControllerDelegate
-  printerPickerControllerWillDismiss(\_:) 

Instance Method

# printerPickerControllerWillDismiss(\_:)

Tells the delegate that the printer picker is about to be dismissed.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func printerPickerControllerWillDismiss(_ printerPickerController: UIPrinterPickerController)
```

## Parameters 

`printerPickerController`  

The printer picker controller object being dismissed.

## Discussion

Use this method to perform any tasks associated with displaying the printer picker controller.

This method is called when the user dismisses the picker, either by selecting a printer or by canceling the picker interface. This method is not called when you dismiss the picker programmatically using the dismiss(animated:) method.

## See Also

### Responding to Printer Picker Events

func printerPickerControllerParentViewController(UIPrinterPickerController) -> UIViewController?

Asks the delegate to provide the view controller to act as the parent of the printer picker.

func printerPickerControllerWillPresent(UIPrinterPickerController)

Tells the delegate that the printer picker is about to be displayed.

func printerPickerControllerDidPresent(UIPrinterPickerController)

Tells the delegate that the printer picker was displayed and is now visible.

func printerPickerControllerDidDismiss(UIPrinterPickerController)

Tells the delegate that the printer picker was dismissed.

