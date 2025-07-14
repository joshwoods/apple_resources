

- AppKit
- NSDocument
-  shouldChangePrintInfo(\_:) 

Instance Method

# shouldChangePrintInfo(\_:)

Returns a Boolean value that indicates whether the document allows changes to the default printing information.

macOS

``` source
@MainActor
func shouldChangePrintInfo(_ newPrintInfo: NSPrintInfo) -> Bool
```

## Parameters 

`newPrintInfo`  

The `NSPrintInfo` object that is the result of the user approving the page layout panel presented by runPageLayout(_:).

## Return Value

true by default; subclasses can override this method to return false.

## Discussion

This method is invoked by the runPageLayout(_:) method, which sets a new `NSPrintInfo`object for the document only if this method returns true.

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

func print(withSettings: [NSPrintInfo.AttributeKey : Any], showPrintPanel: Bool, delegate: Any?, didPrint: Selector?, contextInfo: UnsafeMutableRawPointer?)

Prints the document’s contents, optionally displaying a print panel to the user.

func printOperation(withSettings: [NSPrintInfo.AttributeKey : Any]) throws -> NSPrintOperation

Creates and returns a print operation for the document’s contents.

var pdfPrintOperation: NSPrintOperation

A print operation you can use to create a PDF representation of the document’s current contents.

func saveToPDF(Any?)

Exports a PDF representation of the document’s current contents.

