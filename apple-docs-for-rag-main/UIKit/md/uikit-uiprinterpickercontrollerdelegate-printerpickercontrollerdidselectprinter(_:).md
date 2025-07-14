

- UIKit
- UIPrinterPickerControllerDelegate
-  printerPickerControllerDidSelectPrinter(\_:) 

Instance Method

# printerPickerControllerDidSelectPrinter(\_:)

Tells the delegate that a printer was selected.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func printerPickerControllerDidSelectPrinter(_ printerPickerController: UIPrinterPickerController)
```

## Parameters 

`printerPickerController`  

The printer picker controller that is providing your delegate with information.

## Discussion

Implement this method if you want your delegate to be notified of the selected printer. The selected printer can be either one that the user selected or the initially selected printer that you specified when creating your UIPrinterPickerController object.

