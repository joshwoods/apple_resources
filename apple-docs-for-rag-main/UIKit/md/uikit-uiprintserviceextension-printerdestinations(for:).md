

- UIKit
- UIPrintServiceExtension
-  printerDestinations(for:) 

Instance Method

# printerDestinations(for:)

Searches for a printer destination that matches the print-job attributes.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+visionOS 1.0+

``` source
@MainActor
func printerDestinations(for printInfo: UIPrintInfo) -> [UIPrinterDestination]
```

## Parameters 

`printInfo`  

The characteristics of a print job.

## Return Value

A printer or printers that fulfill the printing options in `printInfo`.

## Discussion

This method inspects the UIPrintInfo record to determine which printers to display to the user.

