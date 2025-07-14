

- Core Graphics
- CGPDFDocument
-  allowsCopying 

Instance Property

# allowsCopying

Returns whether the specified PDF document allows copying.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var allowsCopying: Bool { get }
```

## Discussion

If the document is encrypted and the current password doesn’t grant permission to perform copying, this returns false.

## See Also

### Working with an Encrypted PDF Document

var isEncrypted: Bool

Returns whether the specified PDF file is encrypted.

var allowsPrinting: Bool

Returns whether a PDF document allows printing.

var isUnlocked: Bool

Returns whether the specified PDF document is currently unlocked.

func unlockWithPassword(UnsafePointer&lt;CChar>) -> Bool

Unlocks an encrypted PDF document when a valid password is supplied.

