

- PDFKit
- PDFDocument
- Read Operations
-  Search Operations 

API Collection

# Search Operations

Find and search in PDFs.

## Topics

### Searching Documents

func findString(String, withOptions: NSString.CompareOptions) -> [PDFSelection]

Synchronously finds all instances of the specified string in the document.

func beginFindString(String, withOptions: NSString.CompareOptions)

Asynchronously finds all instances of the specified string in the document.

func beginFindStrings([String], withOptions: NSString.CompareOptions)

Asynchronously finds all instances of the specified array of strings in the document.

func findString(String, fromSelection: PDFSelection?, withOptions: NSString.CompareOptions) -> PDFSelection?

Synchronously finds the next occurance of a string after the specified selection (or before the selection if you specified `NSBackwardsSearch` as a search option.

var isFinding: Bool

Returns a Boolean value indicating whether an asynchronous find operation is in progress.

func cancelFindString()

Cancels a search initiated with beginFindString(_:withOptions:).

## See Also

### Working with Selections and Searches

func selection(from: PDFPage, atCharacterIndex: Int, to: PDFPage, atCharacterIndex: Int) -> PDFSelection?

Returns the specified selection based on starting and ending character indexes.

func selection(from: PDFPage, at: CGPoint, to: PDFPage, at: CGPoint) -> PDFSelection?

Returns the specified selection based on starting and ending points.

var selectionForEntireDocument: PDFSelection?

Returns a selection representing the textual content of the entire document.

