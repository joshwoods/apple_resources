

- PDFKit
-  PDFDocumentWriteOption 

Structure

# PDFDocumentWriteOption

A structure that specifies file writing options for a document.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+macOS 10.4+tvOSvisionOS 1.0+

``` source
struct PDFDocumentWriteOption
```

## Topics

### Creating Write Options

init(rawValue: String)

Initialize a `PDFDocumentWriteOption` structure.

### Getting Write Option Properties

static let ownerPasswordOption: PDFDocumentWriteOption

An `NSString` object for the owner’s password which is required for encryption.

static let userPasswordOption: PDFDocumentWriteOption

An `NSString` object for the user’s password which is optional for encryption.

### Type Properties

static let accessPermissionsOption: PDFDocumentWriteOption

static let burnInAnnotationsOption: PDFDocumentWriteOption

static let optimizeImagesForScreenOption: PDFDocumentWriteOption

static let saveImagesAsJPEGOption: PDFDocumentWriteOption

static let saveTextFromOCROption: PDFDocumentWriteOption

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

struct PDFDocumentAttribute

A structure that specifies document attributes.

