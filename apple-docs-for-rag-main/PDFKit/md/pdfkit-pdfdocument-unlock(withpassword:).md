

- PDFKit
- PDFDocument
-  unlock(withPassword:) 

Instance Method

# unlock(withPassword:)

Attempts to unlock an encrypted document.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
func unlock(withPassword password: String) -> Bool
```

## Parameters 

`password`  

The password to unlock an encrypted document (you cannot lock an unlocked PDF document by using an incorrect password).

## Return Value

true if the specified password unlocks the document, false otherwise.

## Discussion

If the password is correct, this method returns true, and a `PDFDocumentDidUnlockNotification` notification is sent. Once unlocked, you cannot use this function to relock the document.

If you attempt to unlock an already unlocked document, one of the following occurs:

- If the document is unlocked with full owner permissions, `unlockWithPassword` does nothing and returns true. The password string is ignored.

- If the document is unlocked with only user permissions, `unlockWithPassword` attempts to obtain full owner permissions with the password string. If the string fails, the document maintains its user permissions. In either case, this method returns true.

## See Also

### Managing Document Security

var isEncrypted: Bool

A Boolean value specifying whether the document is encrypted.

var isLocked: Bool

A Boolean value indicating whether the document is locked.

var permissionsStatus: PDFDocumentPermissions

The permissions status of the PDF document.

Permission Properties

Properties that specify what functions are allowed for a PDF document.

