

- UIKit
- UIPrinterPickerController
-  init(initiallySelectedPrinter:) 

Initializer

# init(initiallySelectedPrinter:)

Creates and returns a printer picker with an initially selected printer object.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
init(initiallySelectedPrinter printer: UIPrinter?)
```

## Parameters 

`printer`  

A printer object to select initially. Specify `nil` if you do not want to display a selected printer initially.

## Return Value

An initialized printer picker controller object.

## Discussion

After creating a printer picker controller, assign your delegate as needed and present the controller.

