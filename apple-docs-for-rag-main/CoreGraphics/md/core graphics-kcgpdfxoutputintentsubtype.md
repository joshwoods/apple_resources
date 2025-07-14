

- Core Graphics
-  kCGPDFXOutputIntentSubtype 

Global Variable

# kCGPDFXOutputIntentSubtype

The output intent subtype. This key is required.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.4+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
let kCGPDFXOutputIntentSubtype: CFString
```

## Discussion

The value of this key must be a CFString object equal to `"GTS_PDFX"`; otherwise, the dictionary is ignored.

## See Also

### Output Intent Keys

let kCGPDFXOutputConditionIdentifier: CFString

let kCGPDFXOutputCondition: CFString

A text string identifying the intended output device or production condition in a human-readable form.

let kCGPDFXRegistryName: CFString

let kCGPDFXInfo: CFString

let kCGPDFXDestinationOutputProfile: CFString

