

- PDFKit
- PDFDocument
-  permissionsStatus 

Instance Property

# permissionsStatus

The permissions status of the PDF document.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.6+tvOS 11.0+visionOS 1.0+

``` source
var permissionsStatus: PDFDocumentPermissions { get }
```

## See Also

### Managing Document Security

var isEncrypted: Bool

A Boolean value specifying whether the document is encrypted.

var isLocked: Bool

A Boolean value indicating whether the document is locked.

func unlock(withPassword: String) -> Bool

Attempts to unlock an encrypted document.

Permission Properties

Properties that specify what functions are allowed for a PDF document.

