

- AppKit
- NSDocument
-  saveToPDF(\_:) 

Instance Method

# saveToPDF(\_:)

Exports a PDF representation of the document’s current contents.

macOS 10.9+

``` source
@IBAction @MainActor
func saveToPDF(_ sender: Any?)
```

## Parameters 

`sender`  

The control sending the message.

## Discussion

This action method handles the File menu’s “Export As PDF…” item in a document-based application.

The default implementation of this method calls the print(withSettings:showPrintPanel:delegate:didPrint:contextInfo:) method, passing a print settings object that contains only the disposition (save), with user interaction disabled and `NULL` or `nil` for all other parameters.

If your document subclass supports creating PDF representations, you can override this method, if needed.

Important

This method does not copy the document’s printInfo to the operation object when creating a PDF printing operation. Your app should maintain a separate NSPrintInfo instance specifically for creating PDFs and pass it to the print operation’s printInfo method.

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

var pdfPrintOperation: NSPrintOperation

A print operation you can use to create a PDF representation of the document’s current contents.

