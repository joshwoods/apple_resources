

- PDFKit
-  PDFDocumentAttribute 

Structure

# PDFDocumentAttribute

A structure that specifies document attributes.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+macOS 10.4+tvOSvisionOS 1.0+

``` source
struct PDFDocumentAttribute
```

## Topics

### Creating Document Attributes

init(rawValue: String)

Initialize a `PDFDocumentAttribute` structure.

### Getting Document Attributes

static let authorAttribute: PDFDocumentAttribute

An optional text string containing the name of the author of the document.

static let creationDateAttribute: PDFDocumentAttribute

An optional text string containing the document’s creation date.

static let creatorAttribute: PDFDocumentAttribute

An optional text string containing the name of the application that created the document content.

static let keywordsAttribute: PDFDocumentAttribute

An optional array of text strings containing keywords for the document.

static let modificationDateAttribute: PDFDocumentAttribute

An optional text string containing the document’s last-modified date.

static let producerAttribute: PDFDocumentAttribute

An optional text string containing the name of the application that produced the PDF data for the document.

static let subjectAttribute: PDFDocumentAttribute

An optional text string containing a description of the subject of the document.

static let titleAttribute: PDFDocumentAttribute

An optional text string containing the title of the document.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

enum PDFDocumentPermissions

An enumeration that specifies document permissions status.

struct PDFDocumentWriteOption

A structure that specifies file writing options for a document.

