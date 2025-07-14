

- PDFKit
- PDFDocument
-  Write Operations 

API Collection

# Write Operations

Operations that let you write document data to different locations.

## Topics

### Writing Out the PDF Data

func write(toFile: String) -> Bool

Writes the document to a file at the specified path.

func write(toFile: String, withOptions: [PDFDocumentWriteOption : Any]?) -> Bool

Writes the document to a file at the specified path with the specified options.

func write(to: URL) -> Bool

Writes the document to a location specified by the passed-in URL.

func write(to: URL, withOptions: [PDFDocumentWriteOption : Any]?) -> Bool

Writes the document to the specified URL with the specified options.

Data Representations

Operations to represent PDF documents as data objects.

### Printing Documents for macOS

func printOperation(for: NSPrintInfo?, scalingMode: PDFPrintScalingMode, autoRotate: Bool) -> NSPrintOperation?

Returns a print operation suitable for printing the PDF document.

enum PDFPrintScalingMode

The type of scaling to be used when printing a page (see PDFDocument).

## See Also

### Reading and Writing PDFs

Read Operations

Operations that let you access documents and pages, manage document security, and work with searching and selections.

