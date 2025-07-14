

- PDFKit
- PDFDocument
-  Read Operations 

API Collection

# Read Operations

Operations that let you access documents and pages, manage document security, and work with searching and selections.

## Topics

### Accessing Document Information

var documentURL: URL?

The URL for the document.

var majorVersion: Int

The major version of the document.

var minorVersion: Int

The minor version of the document.

var string: String?

A string representing the textual content for the entire document.

func outlineItem(for: PDFSelection) -> PDFOutline?

Returns the most likely parent PDF outline object for the selection.

var outlineRoot: PDFOutline?

The document’s root outline to a PDF outline object.

var documentAttributes: [AnyHashable : Any]?

A dictionary of document metadata.

var documentRef: CGPDFDocument?

The `CGPDFDocument` associated with the `PDFDocument` object.

### Managing Document Security

var isEncrypted: Bool

A Boolean value specifying whether the document is encrypted.

var isLocked: Bool

A Boolean value indicating whether the document is locked.

func unlock(withPassword: String) -> Bool

Attempts to unlock an encrypted document.

var permissionsStatus: PDFDocumentPermissions

The permissions status of the PDF document.

Permission Properties

Properties that specify what functions are allowed for a PDF document.

### Working with Selections and Searches

func selection(from: PDFPage, atCharacterIndex: Int, to: PDFPage, atCharacterIndex: Int) -> PDFSelection?

Returns the specified selection based on starting and ending character indexes.

func selection(from: PDFPage, at: CGPoint, to: PDFPage, at: CGPoint) -> PDFSelection?

Returns the specified selection based on starting and ending points.

var selectionForEntireDocument: PDFSelection?

Returns a selection representing the textual content of the entire document.

Search Operations

Find and search in PDFs.

### Working with Pages

var pageCount: Int

The number of pages in the document.

func page(at: Int) -> PDFPage?

Returns the page at the specified index number.

func index(for: PDFPage) -> Int

Gets the index number for the specified page.

func insert(PDFPage, at: Int)

Inserts a page at the specified index point.

func removePage(at: Int)

Removes the page at the specified index point.

func exchangePage(at: Int, withPageAt: Int)

Swaps one page with another.

var pageClass: AnyClass

The class that is allocated and initialized when page objects are created for the document.

## See Also

### Reading and Writing PDFs

Write Operations

Operations that let you write document data to different locations.

