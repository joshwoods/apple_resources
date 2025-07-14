

- AppKit
-  NSPrintOperation 

Class

# NSPrintOperation

An object that controls operations that generate Encapsulated PostScript (EPS) code, Portable Document Format (PDF) code, or print jobs.

macOS

``` source
@MainActor
class NSPrintOperation
```

## Overview

An NSPrintOperation object works in conjunction with two other objects: an NSPrintInfo object, which specifies how the code should be generated, and an NSView object, which generates the actual code.

It is important to note that the majority of methods in NSPrintOperation copy the instance of NSPrintInfo passed into them. Future changes to that print info are not reflected in the print info retained by the current NSPrintOperation object. All changes should be made to the print info before passing to the methods of this class. The only method in NSPrintOperation which does not copy the NSPrintInfo instance is printInfo.

Note

You should not subclass NSPrintOperation. Methods that return a print operation object return an instance of a concrete subclass whose implementation is private.

## Topics

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

init(view: NSView, printInfo: NSPrintInfo)

Creates and returns an print operation object ready to control the printing of the specified view using custom print settings.

### Setting the Current Print Operation for This Thread

class var current: NSPrintOperation?

The current print operation for this thread.

### Determining the Type of Operation

var isCopyingOperation: Bool

A Boolean value that indicates whether the print operation is an EPS or PDF copy operation.

### Modifying the Printing Information

var printInfo: NSPrintInfo

The printing information associated with the print operation.

class NSPrintInfo

An object that stores information that’s used to generate printed output.

### Getting the View

var view: NSView?

The view object that generates the actual data for the print operation.

### Getting the Printing Quality

var preferredRenderingQuality: NSPrintOperation.RenderingQuality

The printing quality.

enum RenderingQuality

Constants that specify the print quality in use.

### Running the Print Operation

func run() -> Bool

Runs the print operation on the current thread.

func runModal(for: NSWindow, delegate: Any?, didRun: Selector?, contextInfo: UnsafeMutableRawPointer?)

Runs the print operation, calling your custom delegate method upon completion.

func cleanUp()

Called at the end of a print operation to remove the print operation as the current operation.

func deliverResult() -> Bool

Delivers the results of the print operation to the intended destination.

### Modifying the User Interface

var showsPrintPanel: Bool

A Boolean value that determines whether the print operation displays a print panel.

var showsProgressPanel: Bool

A Boolean value that determines whether the print operation displays a progress panel.

var jobTitle: String?

The custom title of the print job.

var printPanel: NSPrintPanel

The print panel object to use during the operation.

var pdfPanel: NSPDFPanel

The PDF panel object to use during the operation.

### Managing the Drawing Context

var context: NSGraphicsContext?

The graphics context object used for generating output.

func createContext() -> NSGraphicsContext?

Creates the graphics context object used for drawing during the operation.

func destroyContext()

Destroys the print operation’s graphics context.

### Managing Page Information

var currentPage: Int

The current page number being printed.

var pageRange: NSRange

The range of pages associated with the print operation.

var pageOrder: NSPrintOperation.PageOrder

The print order for the pages of the operation.

enum PageOrder

Constants that specify the page order.

### Managing Printing Threads

var canSpawnSeparateThread: Bool

A Boolean value that determines whether the print operation is allowed to spawn a separate printing thread.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Print Information

class NSPrinter

An object that describes a printer’s capabilities.

class NSPrintInfo

An object that stores information that’s used to generate printed output.

