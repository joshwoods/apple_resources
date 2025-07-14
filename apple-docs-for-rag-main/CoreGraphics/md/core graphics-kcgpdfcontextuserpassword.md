

- Core Graphics
-  kCGPDFContextUserPassword 

Global Variable

# kCGPDFContextUserPassword

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
let kCGPDFContextUserPassword: CFString
```

## Discussion

The user password of the PDF document. If the document is encrypted, then the value of this key will be the user password for the document. If not specified, the user password is the empty string. The value of this key must be a CFString object that can be represented in ASCII encoding; only the first 32 bytes will be used for the password. If the value of this key cannot be represented in ASCII, the document is not created and the creation function returns `NULL`.

## See Also

### Metadata Keys

let kCGPDFContextAuthor: CFString

The corresponding value is a string that represents the name of the person who created the document. This key is optional.

let kCGPDFContextCreator: CFString

The corresponding value is a string that represents the name of the application used to produce the document. This key is optional.

let kCGPDFContextTitle: CFString

The corresponding value is a string that represents the title of the document. This key is optional.

let kCGPDFContextOwnerPassword: CFString

let kCGPDFContextAllowsPrinting: CFString

Whether the document allows printing when unlocked with the user password.

let kCGPDFContextAllowsCopying: CFString

Whether the document allows copying when unlocked with the user password.

let kCGPDFContextOutputIntent: CFString

let kCGPDFContextOutputIntents: CFString

let kCGPDFContextSubject: CFString

let kCGPDFContextKeywords: CFString

let kCGPDFContextEncryptionKeyLength: CFString

