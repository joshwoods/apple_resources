

- Core Graphics
-  kCGPDFContextAllowsPrinting 

Global Variable

# kCGPDFContextAllowsPrinting

Whether the document allows printing when unlocked with the user password.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
let kCGPDFContextAllowsPrinting: CFString
```

## Discussion

The value of this key must be a CFBoolean value. The default value of this key is true.

## See Also

### Metadata Keys

let kCGPDFContextAuthor: CFString

The corresponding value is a string that represents the name of the person who created the document. This key is optional.

let kCGPDFContextCreator: CFString

The corresponding value is a string that represents the name of the application used to produce the document. This key is optional.

let kCGPDFContextTitle: CFString

The corresponding value is a string that represents the title of the document. This key is optional.

let kCGPDFContextOwnerPassword: CFString

let kCGPDFContextUserPassword: CFString

let kCGPDFContextAllowsCopying: CFString

Whether the document allows copying when unlocked with the user password.

let kCGPDFContextOutputIntent: CFString

let kCGPDFContextOutputIntents: CFString

let kCGPDFContextSubject: CFString

let kCGPDFContextKeywords: CFString

let kCGPDFContextEncryptionKeyLength: CFString

