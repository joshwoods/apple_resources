

- Core Graphics
-  kCGPDFContextKeywords 

Global Variable

# kCGPDFContextKeywords

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
let kCGPDFContextKeywords: CFString
```

## Discussion

The keywords for this document. This key is optional. If the value of this key is a CFString object, the `/Keywords` entry will be the specified string. If the value of this key is a CFArray object, then it must be an array of CFString objects. The `/Keywords` entry will, in this case, be the concatenation of the specified strings separated by commas (`","`). In addition, an entry with the key `"/AAPL:Keywords"` is stored in the document information dictionary; its value is an array consisting of each of the specified strings. The value of this key must be in one of the above forms; otherwise, this key is ignored.

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

let kCGPDFContextAllowsPrinting: CFString

Whether the document allows printing when unlocked with the user password.

let kCGPDFContextAllowsCopying: CFString

Whether the document allows copying when unlocked with the user password.

let kCGPDFContextOutputIntent: CFString

let kCGPDFContextOutputIntents: CFString

let kCGPDFContextSubject: CFString

let kCGPDFContextEncryptionKeyLength: CFString

