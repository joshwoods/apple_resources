

- AppKit
- NSPrintOperation
-  init(view:printInfo:) 

Initializer

# init(view:printInfo:)

Creates and returns an print operation object ready to control the printing of the specified view using custom print settings.

macOS

``` source
@MainActor
init(
    view: NSView,
    printInfo: NSPrintInfo
)
```

## Parameters 

`view`  

The view whose contents you want to print.

`printInfo`  

The print settings to use when printing the view.

## Return Value

The new `NSPrintOperation` object. You must run the operation to print the view.

## Discussion

This method raises an `NSPrintOperationExistsException` if there is already a print operation in progress; otherwise the returned object is made the current print operation for this thread.

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

init(view: NSView)

Creates and returns an print operation object ready to control the printing of the specified view.

