

- Core Graphics
- CGPDFDocument
-  unlockWithPassword(\_:) 

Instance Method

# unlockWithPassword(\_:)

Unlocks an encrypted PDF document when a valid password is supplied.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func unlockWithPassword(_ password: UnsafePointer) -> Bool
```

## Parameters 

`password`  

A pointer to a string that contains the password.

## Return Value

A Boolean that, if true, indicates that the document has been successfully unlocked. If the value is false, the document has not been unlocked.

## Discussion

Given an encrypted PDF document and a password, this function does the following:

- Sets the lock state of the document, based on the validity of the password.

- Returns true if the document is unlocked.

- Returns false if the document cannot be unlocked with the specified password.

Unlocking a PDF document makes it possible to decrypt the document and perform other privileged operations. Different passwords enable different operations.

## See Also

### Working with an Encrypted PDF Document

var isEncrypted: Bool

Returns whether the specified PDF file is encrypted.

var allowsCopying: Bool

Returns whether the specified PDF document allows copying.

var allowsPrinting: Bool

Returns whether a PDF document allows printing.

var isUnlocked: Bool

Returns whether the specified PDF document is currently unlocked.

