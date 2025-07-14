

- UIKit
- UIPrinterPickerControllerDelegate
-  printerPickerControllerWillPresent(\_:) 

Instance Method

# printerPickerControllerWillPresent(\_:)

Tells the delegate that the printer picker is about to be displayed.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func printerPickerControllerWillPresent(_ printerPickerController: UIPrinterPickerController)
```

## Parameters 

`printerPickerController`  

The printer picker controller object being displayed.

## Discussion

Use this method to perform any tasks associated with displaying the printer picker controller.

## See Also

### Responding to Printer Picker Events

func printerPickerControllerParentViewController(UIPrinterPickerController) -> UIViewController?

Asks the delegate to provide the view controller to act as the parent of the printer picker.

func printerPickerControllerDidPresent(UIPrinterPickerController)

Tells the delegate that the printer picker was displayed and is now visible.

func printerPickerControllerWillDismiss(UIPrinterPickerController)

Tells the delegate that the printer picker is about to be dismissed.

func printerPickerControllerDidDismiss(UIPrinterPickerController)

Tells the delegate that the printer picker was dismissed.

