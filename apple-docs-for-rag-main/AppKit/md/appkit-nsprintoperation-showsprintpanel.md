

- AppKit
- NSPrintOperation
-  showsPrintPanel 

Instance Property

# showsPrintPanel

A Boolean value that determines whether the print operation displays a print panel.

macOS

``` source
@MainActor
var showsPrintPanel: Bool { get set }
```

## Parameters 

`flag`  

true if you want to display a print panel; otherwise, false.

## Discussion

This method does not affect the display of a progress panel; that operation is controlled by the showsProgressPanel method.

Operations that generate EPS or PDF data do no display a progress panel, regardless of the value in the `flag` parameter.

## See Also

### Modifying the User Interface

var showsProgressPanel: Bool

A Boolean value that determines whether the print operation displays a progress panel.

var jobTitle: String?

The custom title of the print job.

var printPanel: NSPrintPanel

The print panel object to use during the operation.

var pdfPanel: NSPDFPanel

The PDF panel object to use during the operation.

