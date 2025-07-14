

- AppKit
- NSDocument
-  printOperation(withSettings:) 

Instance Method

# printOperation(withSettings:)

Creates and returns a print operation for the document’s contents.

macOS

``` source
@MainActor
func printOperation(withSettings printSettings: [NSPrintInfo.AttributeKey : Any]) throws -> NSPrintOperation
```

## Parameters 

`printSettings`  

The print settings dictionary to use.

## Return Value

The print operation, or `nil` if unsuccessful.

## Discussion

The print operation can be run to print the document’s current contents. The `NSPrintInfo` attributes in the passed-in `printSettings` dictionary are added to a copy of the document’s print info, and the resulting print info is used for the operation.

Important

You must override this method to enable printing in your app. The default implementation raises an exception.

Handling Errors in Swift

In Swift, this method is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

When overriding this method, use the `throw` statement to throw an `NSError`, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

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

var pdfPrintOperation: NSPrintOperation

A print operation you can use to create a PDF representation of the document’s current contents.

func saveToPDF(Any?)

Exports a PDF representation of the document’s current contents.

