

- UIKit
- UIPrinterPickerController
-  selectedPrinter 

Instance Property

# selectedPrinter

The selected printer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var selectedPrinter: UIPrinter? { get }
```

## Discussion

The value of this property is set to the picker you specified at creation time initially. When the picker is dismissed, the value is updated to reflect the printer that the user selected, if any. If the user cancels the picker without selecting a printer, the value of this property does not change.

