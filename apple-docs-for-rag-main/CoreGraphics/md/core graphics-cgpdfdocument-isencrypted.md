

- Core Graphics
- CGPDFDocument
-  isEncrypted 

Instance Property

# isEncrypted

Returns whether the specified PDF file is encrypted.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var isEncrypted: Bool { get }
```

## Discussion

If the document is encrypted, a password must be supplied before certain operations are enabled. For more information, see unlockWithPassword(_:).

## See Also

### Working with an Encrypted PDF Document

var allowsCopying: Bool

Returns whether the specified PDF document allows copying.

var allowsPrinting: Bool

Returns whether a PDF document allows printing.

var isUnlocked: Bool

Returns whether the specified PDF document is currently unlocked.

func unlockWithPassword(UnsafePointer&lt;CChar>) -> Bool

Unlocks an encrypted PDF document when a valid password is supplied.

