

- Core Graphics
-  kCGPDFContextOutputIntent 

Global Variable

# kCGPDFContextOutputIntent

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.4+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
let kCGPDFContextOutputIntent: CFString
```

## Discussion

The output intent `PDF/X`. This key is optional. If present, the value of this key must be a CFDictionary object. The dictionary is added to the `/OutputIntents` entry in the PDF file document catalog. The keys and values contained in the dictionary must match those specified in section 9.10.4 of the PDF 1.4 specification, ISO/DIS 15930-3 document published by ISO/TC 130, and Adobe Technical Note \#5413.

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

let kCGPDFContextOutputIntents: CFString

let kCGPDFContextSubject: CFString

let kCGPDFContextKeywords: CFString

let kCGPDFContextEncryptionKeyLength: CFString

