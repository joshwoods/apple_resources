

- AppKit
- NSPrintOperation
-  epsOperation(with:inside:toPath:printInfo:) 

Type Method

# epsOperation(with:inside:toPath:printInfo:)

Creates and returns a new print operation object ready to control the copying of EPS graphics from the specified view and write the resulting data to the specified file.

macOS

``` source
@MainActor
class func epsOperation(
    with view: NSView,
    inside rect: NSRect,
    toPath path: String,
    printInfo: NSPrintInfo
) -> NSPrintOperation
```

## Parameters 

`view`  

The view containing the data to be turned into EPS data.

`rect`  

The portion of the view (specified in points in the view’s coordinate space) to be rendered as EPS data.

`path`  

The path to a file. After the job is run, this file contains the EPS data.

`printInfo`  

The print settings to use when generating the EPS data.

## Return Value

The new `NSPrintOperation` object. You must run the operation to generate the EPS data.

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

class func pdfOperation(with: NSView, inside: NSRect, to: NSMutableData) -> NSPrintOperation

Creates and returns a new print operation object ready to control the copying of PDF graphics from the specified view.

class func pdfOperation(with: NSView, inside: NSRect, to: NSMutableData, printInfo: NSPrintInfo) -> NSPrintOperation

Creates and returns a new print operation object ready to control the copying of PDF graphics from the specified view using the specified print settings.

class func pdfOperation(with: NSView, inside: NSRect, toPath: String, printInfo: NSPrintInfo) -> NSPrintOperation

Creates and returns a new print operation object ready to control the copying of PDF graphics from the specified view and write the resulting data to the specified file.

init(view: NSView)

Creates and returns an print operation object ready to control the printing of the specified view.

init(view: NSView, printInfo: NSPrintInfo)

Creates and returns an print operation object ready to control the printing of the specified view using custom print settings.

