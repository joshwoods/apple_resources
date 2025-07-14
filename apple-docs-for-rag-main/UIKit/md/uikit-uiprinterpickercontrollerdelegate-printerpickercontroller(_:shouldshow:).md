

- UIKit
- UIPrinterPickerControllerDelegate
-  printerPickerController(\_:shouldShow:) 

Instance Method

# printerPickerController(\_:shouldShow:)

Asks the delegate if the specified printer should be included in the picker.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func printerPickerController(
    _ printerPickerController: UIPrinterPickerController,
    shouldShow printer: UIPrinter
) -> Bool
```

## Parameters 

`printerPickerController`  

The printer picker controller that is asking the delegate for information.

`printer`  

The printer object for the delegate to consider.

## Return Value

true if the printer should be displayed or false if it should not.

## Discussion

Implement this method in your delegate if you want to filter the list of printers displayed by the printer picker interface. You might use this method to display only printers with specific capabilities. The printer picker interface calls this method once for each printer it is preparing to display, so your implementation should perform any required checks and return as quickly as possible. Do not perform any lengthy operations in this method.

If you do not implement this method, the picker interface displays all of the printers that it finds.

