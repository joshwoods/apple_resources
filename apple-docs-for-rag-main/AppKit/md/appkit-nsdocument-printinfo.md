

- AppKit
- NSDocument
-  printInfo 

Instance Property

# printInfo

The printing information associated with the document.

macOS

``` source
@NSCopying @MainActor
var printInfo: NSPrintInfo { get set }
```

## Return Value

The receiver’s `NSPrintInfo` object.

## Discussion

The default value of this property is the default NSPrintInfo object. To customize the printing information, assign a new value to this property. The Page Layout panel may also update the object in this property to reflect the options selected by the user.

## See Also

### Related Documentation

func runPageLayout(Any?)

The action method invoked in the receiver as first responder when the user chooses the Page Setup menu command.

### Printing the Document

func preparePageLayout(NSPageLayout) -> Bool

Adds document-specific content to the Page Layout panel.

func runModalPageLayout(with: NSPrintInfo, delegate: Any?, didRun: Selector?, contextInfo: UnsafeMutableRawPointer?)

Runs the modal page layout panel with the receiver’s printing information object.

func runModalPrintOperation(NSPrintOperation, delegate: Any?, didRun: Selector?, contextInfo: UnsafeMutableRawPointer?)

Runs the specified print operation modally.

func shouldChangePrintInfo(NSPrintInfo) -> Bool

Returns a Boolean value that indicates whether the document allows changes to the default printing information.

func print(withSettings: [NSPrintInfo.AttributeKey : Any], showPrintPanel: Bool, delegate: Any?, didPrint: Selector?, contextInfo: UnsafeMutableRawPointer?)

Prints the document’s contents, optionally displaying a print panel to the user.

func printOperation(withSettings: [NSPrintInfo.AttributeKey : Any]) throws -> NSPrintOperation

Creates and returns a print operation for the document’s contents.

var pdfPrintOperation: NSPrintOperation

A print operation you can use to create a PDF representation of the document’s current contents.

func saveToPDF(Any?)

Exports a PDF representation of the document’s current contents.

