

- UIKit
- UIPrinterPickerControllerDelegate
-  printerPickerControllerDidDismiss(\_:) 

Instance Method

# printerPickerControllerDidDismiss(\_:)

Tells the delegate that the printer picker was dismissed.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func printerPickerControllerDidDismiss(_ printerPickerController: UIPrinterPickerController)
```

## Parameters 

`printerPickerController`  

The printer picker controller object that was dismissed.

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

func printerPickerControllerWillDismiss(UIPrinterPickerController)

Tells the delegate that the printer picker is about to be dismissed.

