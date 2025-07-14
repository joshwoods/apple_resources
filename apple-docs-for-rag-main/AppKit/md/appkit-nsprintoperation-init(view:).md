

- AppKit
- NSPrintOperation
-  init(view:) 

Initializer

# init(view:)

Creates and returns an print operation object ready to control the printing of the specified view.

macOS

``` source
@MainActor
init(view: NSView)
```

## Parameters 

`view`  

The view whose contents you want to print.

## Return Value

The new `NSPrintOperation` object. You must run the operation to print the view.

## Discussion

The new `NSPrintOperation` object uses the settings stored in the shared `NSPrintInfo` object. This method raises an `NSPrintOperationExistsException` if there is already a print operation in progress; otherwise the returned object is made the current print operation for this thread.

## See Also

### Related Documentation

func run() -> Bool

Runs the print operation on the current thread.

### Creating the Printing Operation Object

class func epsOperation(with: NSView, inside: NSRect, to: NSMutableData?) -> NSPrintOperation

Creates and returns a new print operation object ready to control the copying of EPS graphics from the specified view.

class func epsOperation(with: NSView, inside: NSRect, to: NSMutableData, printInfo: NSPrintInfo) -> NSPrintOperation

Creates and returns a new print operation object ready to control the copying of EPS graphics from the specified view using the specified print settings.

class func epsOperation(with: NSView, inside: NSRect, toPath: String, printInfo: NSPrintInfo) -> NSPrintOperation

Creates and returns a new print operation object ready to control the copying of EPS graphics from the specified view and write the resulting data to the specified file.

class func pdfOperation(with: NSView, inside: NSRect, to: NSMutableData) -> NSPrintOperation

Creates and returns a new print operation object ready to control the copying of PDF graphics from the specified view.

class func pdfOperation(with: NSView, inside: NSRect, to: NSMutableData, printInfo: NSPrintInfo) -> NSPrintOperation

Creates and returns a new print operation object ready to control the copying of PDF graphics from the specified view using the specified print settings.

class func pdfOperation(with: NSView, inside: NSRect, toPath: String, printInfo: NSPrintInfo) -> NSPrintOperation

Creates and returns a new print operation object ready to control the copying of PDF graphics from the specified view and write the resulting data to the specified file.

init(view: NSView, printInfo: NSPrintInfo)

Creates and returns an print operation object ready to control the printing of the specified view using custom print settings.

