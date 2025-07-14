

- PDFKit
- PDFDocument
-  isLocked 

Instance Property

# isLocked

A Boolean value indicating whether the document is locked.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
var isLocked: Bool { get }
```

## Return Value

true if the document is locked; false otherwise.

## Discussion

Only encrypted documents can be locked. Encrypted documents whose password is the empty string are unlocked automatically upon opening, because PDF Kit tries the empty string as a password if none is supplied. Use the unlock(withPassword:) method to unlock a document using a password.

## See Also

### Managing Document Security

var isEncrypted: Bool

A Boolean value specifying whether the document is encrypted.

func unlock(withPassword: String) -> Bool

Attempts to unlock an encrypted document.

var permissionsStatus: PDFDocumentPermissions

The permissions status of the PDF document.

Permission Properties

Properties that specify what functions are allowed for a PDF document.

