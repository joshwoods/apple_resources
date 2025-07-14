

- Core Graphics
- CGPDFDocument
-  isUnlocked 

Instance Property

# isUnlocked

Returns whether the specified PDF document is currently unlocked.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var isUnlocked: Bool { get }
```

## Discussion

There are two possible reasons why a PDF document is unlocked:

- The document is not encrypted.

- The document is encrypted, and a valid password was previously specified using unlockWithPassword(_:).

## See Also

### Working with an Encrypted PDF Document

var isEncrypted: Bool

Returns whether the specified PDF file is encrypted.

var allowsCopying: Bool

Returns whether the specified PDF document allows copying.

var allowsPrinting: Bool

Returns whether a PDF document allows printing.

func unlockWithPassword(UnsafePointer&lt;CChar>) -> Bool

Unlocks an encrypted PDF document when a valid password is supplied.

