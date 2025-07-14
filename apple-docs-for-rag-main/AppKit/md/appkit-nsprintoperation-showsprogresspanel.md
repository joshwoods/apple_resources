

- AppKit
- NSPrintOperation
-  showsProgressPanel 

Instance Property

# showsProgressPanel

A Boolean value that determines whether the print operation displays a progress panel.

macOS

``` source
@MainActor
var showsProgressPanel: Bool { get set }
```

## Parameters 

`flag`  

true if you want to display a progress panel; otherwise, false.

## Discussion

This method does not affect the display of a print panel; that operation is controlled by the showsPrintPanel method.

Operations that generate EPS or PDF data do no display a progress panel, regardless of the value in the `flag` parameter.

## See Also

### Modifying the User Interface

var showsPrintPanel: Bool

A Boolean value that determines whether the print operation displays a print panel.

var jobTitle: String?

The custom title of the print job.

var printPanel: NSPrintPanel

The print panel object to use during the operation.

var pdfPanel: NSPDFPanel

The PDF panel object to use during the operation.

