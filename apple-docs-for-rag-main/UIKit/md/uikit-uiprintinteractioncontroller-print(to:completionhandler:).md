

- UIKit
- UIPrintInteractionController
-  print(to:completionHandler:) 

Instance Method

# print(to:completionHandler:)

Prints directly to the specified printer.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func print(
    to printer: UIPrinter,
    completionHandler completion: UIPrintInteractionController.CompletionHandler? = nil
) -> Bool
```

## Parameters 

`printer`  

The printer to use for printing. You can obtain a list of available printers using a UIPrinterPickerController object.

`completion`  

The block to execute when the print operation finishes.

## Return Value

true if printing was successful or false if there was a problem.

## Discussion

This method starts the print job and displays the printing progress indicator to the user. This method associates the current printing information (available in the printInfo property) with the job but disables duplex printing. Upon completion of the print job, the print interaction controller executes the block in the `completion` parameter.

## See Also

### Printing directly to a printer

typealias CompletionHandler

A completion handler for responding to the completion of a print job or for handling printing errors.

