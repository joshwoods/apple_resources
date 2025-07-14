

- Core Graphics
-  kCGPDFContextOwnerPassword 

Global Variable

# kCGPDFContextOwnerPassword

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
let kCGPDFContextOwnerPassword: CFString
```

## Discussion

The owner password of the PDF document. If this key is specified, the document is encrypted using the value as the owner password; otherwise, the document will not be encrypted. The value of this key must be a CFString object that can be represented in ASCII encoding. Only the first 32 bytes are used for the password. There is no default value for this key. If the value of this key cannot be represented in ASCII, the document is not created and the creation function returns `NULL`.

## See Also

### Metadata Keys

let kCGPDFContextAuthor: CFString

The corresponding value is a string that represents the name of the person who created the document. This key is optional.

let kCGPDFContextCreator: CFString

The corresponding value is a string that represents the name of the application used to produce the document. This key is optional.

let kCGPDFContextTitle: CFString

The corresponding value is a string that represents the title of the document. This key is optional.

let kCGPDFContextUserPassword: CFString

let kCGPDFContextAllowsPrinting: CFString

Whether the document allows printing when unlocked with the user password.

let kCGPDFContextAllowsCopying: CFString

Whether the document allows copying when unlocked with the user password.

let kCGPDFContextOutputIntent: CFString

let kCGPDFContextOutputIntents: CFString

let kCGPDFContextSubject: CFString

let kCGPDFContextKeywords: CFString

let kCGPDFContextEncryptionKeyLength: CFString

