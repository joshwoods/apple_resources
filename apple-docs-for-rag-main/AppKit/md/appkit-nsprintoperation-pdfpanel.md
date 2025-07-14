

- AppKit
- NSPrintOperation
-  pdfPanel 

Instance Property

# pdfPanel

The PDF panel object to use during the operation.

macOS 10.9+

``` source
@MainActor
var pdfPanel: NSPDFPanel { get set }
```

## See Also

### Modifying the User Interface

var showsPrintPanel: Bool

A Boolean value that determines whether the print operation displays a print panel.

var showsProgressPanel: Bool

A Boolean value that determines whether the print operation displays a progress panel.

var jobTitle: String?

The custom title of the print job.

var printPanel: NSPrintPanel

The print panel object to use during the operation.

