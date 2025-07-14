

- AppKit
- NSPrintOperation
-  printPanel 

Instance Property

# printPanel

The print panel object to use during the operation.

macOS

``` source
@MainActor
var printPanel: NSPrintPanel { get set }
```

## Parameters 

`panel`  

The print panel object to use for the operation.

## See Also

### Modifying the User Interface

var showsPrintPanel: Bool

A Boolean value that determines whether the print operation displays a print panel.

var showsProgressPanel: Bool

A Boolean value that determines whether the print operation displays a progress panel.

var jobTitle: String?

The custom title of the print job.

var pdfPanel: NSPDFPanel

The PDF panel object to use during the operation.

