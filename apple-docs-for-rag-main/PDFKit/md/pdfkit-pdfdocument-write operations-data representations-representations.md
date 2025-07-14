

- PDFKit
- PDFDocument
- Write Operations
-  Data Representations 

API Collection

# Data Representations

Operations to represent PDF documents as data objects.

## Topics

### Creating Data Representations

func dataRepresentation() -> Data?

Returns a representation of the document as an `NSData` object.

func dataRepresentation(options: [AnyHashable : Any]) -> Data?

Returns a representation of the document as an `NSData` object with additional options applied, such as filters.

## See Also

### Writing Out the PDF Data

func write(toFile: String) -> Bool

Writes the document to a file at the specified path.

func write(toFile: String, withOptions: [PDFDocumentWriteOption : Any]?) -> Bool

Writes the document to a file at the specified path with the specified options.

func write(to: URL) -> Bool

Writes the document to a location specified by the passed-in URL.

func write(to: URL, withOptions: [PDFDocumentWriteOption : Any]?) -> Bool

Writes the document to the specified URL with the specified options.

