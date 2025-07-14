

- AppKit
- NSDocument
-  preparePageLayout(\_:) 

Instance Method

# preparePageLayout(\_:)

Adds document-specific content to the Page Layout panel.

macOS

``` source
@MainActor
func preparePageLayout(_ pageLayout: NSPageLayout) -> Bool
```

## Parameters 

`pageLayout`  

The page layout panel to prepare.

## Return Value

true if successfully prepared; otherwise, false.

## Discussion

The runModalPageLayoutWithPrintInfo: and runModalPageLayout(with:delegate:didRun:contextInfo:) methods call this method to allow the document to customize the Page Layout panel `pageLayout`. You might use this method to add a document-related accessory view.

The default implementation returns true.

## See Also

### Printing the Document

var printInfo: NSPrintInfo

The printing information associated with the document.

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

