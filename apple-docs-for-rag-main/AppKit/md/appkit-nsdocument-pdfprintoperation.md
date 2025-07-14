

- AppKit
- NSDocument
-  pdfPrintOperation 

Instance Property

# pdfPrintOperation

A print operation you can use to create a PDF representation of the document’s current contents.

macOS 10.9+

``` source
@MainActor
var pdfPrintOperation: NSPrintOperation { get }
```

## Discussion

The object in this property can be run to print the document’s current contents to a PDF file.

The default print operation stored by this property is obtained by calling the printOperation(withSettings:) method and passing a print settings object that contains only the disposition (save) and a `NULL` error object reference. If your document subclass supports creating PDF representations, you can override this property as needed to customize the options.

Important

This property does not copy the document’s printInfo to the PDF printing operation object. Your app should maintain a separate NSPrintInfo instance specifically for creating PDFs and assign it to the printInfo property of the operation object.

## See Also

### Printing the Document

var printInfo: NSPrintInfo

The printing information associated with the document.

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

func saveToPDF(Any?)

Exports a PDF representation of the document’s current contents.

