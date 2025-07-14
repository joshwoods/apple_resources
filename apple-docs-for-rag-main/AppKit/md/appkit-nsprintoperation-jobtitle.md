

- AppKit
- NSPrintOperation
-  jobTitle 

Instance Property

# jobTitle

The custom title of the print job.

macOS 10.5+

``` source
@MainActor
var jobTitle: String? { get set }
```

## Parameters 

`jobTitle`  

The print job title. The receiver makes its own copy of the specified string.

## Discussion

Assigning a title with this method overrides the job title provided by the printing view’s printJobTitle method. Specifying `nil` for the `jobTitle` parameter causes the receiver to once again take its title from the printing view.

## See Also

### Related Documentation

var printJobTitle: String

The view’s print job title.

### Modifying the User Interface

var showsPrintPanel: Bool

A Boolean value that determines whether the print operation displays a print panel.

var showsProgressPanel: Bool

A Boolean value that determines whether the print operation displays a progress panel.

var printPanel: NSPrintPanel

The print panel object to use during the operation.

var pdfPanel: NSPDFPanel

The PDF panel object to use during the operation.

