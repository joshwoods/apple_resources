

- UIKit
- UIPrinterPickerController
-  UIPrinterPickerController.CompletionHandler 

Type Alias

# UIPrinterPickerController.CompletionHandler

The completion handler to execute when dismissing a printer picker controller.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
typealias CompletionHandler = (UIPrinterPickerController, Bool, (any Error)?) -> Void
```

## Discussion

A printer picker completion handler takes the following parameters:

printerPickerController  
The printer picker controller object that is being dismissed. This parameter contains information about the selected printer, if any.

userDidSelect  
true if the user selected a printer or false if the user canceled the selection process. When this parameter is true, use the `printerPickerController` object to retrieve the selected printer object.

error  
An NSError object if there was a problem with the printer picker or `nil` if a printer was selected or the user canceled the picker.

