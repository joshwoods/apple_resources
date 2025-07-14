

- PDFKit
- PDFDocument
- Read Operations
-  Permission Properties 

API Collection

# Permission Properties

Properties that specify what functions are allowed for a PDF document.

## Topics

### Getting Permissions

var allowsCopying: Bool

A Boolean value indicating whether the document allows copying of content to the Pasteboard.

var allowsPrinting: Bool

A Boolean value indicating whether the document allows printing.

var allowsCommenting: Bool

A Boolean value indicating whether you can create or modify document annotations, including form field entries.

var allowsContentAccessibility: Bool

A Boolean value indicating whether you can extract content from the document, but only for the purpose of accessibility.

var allowsDocumentAssembly: Bool

A Boolean value indicating whether you can manage a document by inserting, deleting, and rotating pages.

var allowsDocumentChanges: Bool

A Boolean value indicating whether you can modify the document contents except for document attributes.

var allowsFormFieldEntry: Bool

A Boolean value indicating whether you can modify form field entries even if you can’t edit document annotations.

## See Also

### Managing Document Security

var isEncrypted: Bool

A Boolean value specifying whether the document is encrypted.

var isLocked: Bool

A Boolean value indicating whether the document is locked.

func unlock(withPassword: String) -> Bool

Attempts to unlock an encrypted document.

var permissionsStatus: PDFDocumentPermissions

The permissions status of the PDF document.

