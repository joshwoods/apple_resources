

- UIKit
- UIPrinterPickerControllerDelegate
-  printerPickerControllerParentViewController(\_:) 

Instance Method

# printerPickerControllerParentViewController(\_:)

Asks the delegate to provide the view controller to act as the parent of the printer picker.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func printerPickerControllerParentViewController(_ printerPickerController: UIPrinterPickerController) -> UIViewController?
```

## Parameters 

`printerPickerController`  

The printer picker controller object that made the request.

## Return Value

A view controller from your app’s interface.

## Discussion

Use this method when you want the printer picker controller to be presented from a specific view controller in your app’s interface. When you specify a navigation controller as the parent, UIKit pushes the printer picker onto your navigation stack. For other types of view controllers, UIKit presents the picker interface from the view controller you specify.

If you do not implement this method or your implementation returns `nil`, UIKit presents the printer picker from the root view controller of your app’s main window.

## See Also

### Responding to Printer Picker Events

func printerPickerControllerWillPresent(UIPrinterPickerController)

Tells the delegate that the printer picker is about to be displayed.

func printerPickerControllerDidPresent(UIPrinterPickerController)

Tells the delegate that the printer picker was displayed and is now visible.

func printerPickerControllerWillDismiss(UIPrinterPickerController)

Tells the delegate that the printer picker is about to be dismissed.

func printerPickerControllerDidDismiss(UIPrinterPickerController)

Tells the delegate that the printer picker was dismissed.

