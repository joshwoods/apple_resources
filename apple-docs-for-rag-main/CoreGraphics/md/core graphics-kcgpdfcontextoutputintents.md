

- Core Graphics
-  kCGPDFContextOutputIntents 

Global Variable

# kCGPDFContextOutputIntents

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.4+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
let kCGPDFContextOutputIntents: CFString
```

## Discussion

Output intent dictionaries. This key is optional. If present, the value must be an array of one or more kCGPDFContextOutputIntent dictionaries. The array is added to the PDF document in the `/OutputIntents` entry in the PDF file’s document catalog. Each dictionary in the array must be of form specified for the kCGPDFContextOutputIntent key, except that only the first dictionary in the array is required to contain the “S” key with a value of `GTS_PDFX`. If both the kCGPDFContextOutputIntent and kCGPDFContextOutputIntents keys are specified, the former is ignored.

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

let kCGPDFContextSubject: CFString

let kCGPDFContextKeywords: CFString

let kCGPDFContextEncryptionKeyLength: CFString

