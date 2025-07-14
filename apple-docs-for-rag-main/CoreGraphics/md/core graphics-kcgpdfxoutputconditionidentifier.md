

- Core Graphics
-  kCGPDFXOutputConditionIdentifier 

Global Variable

# kCGPDFXOutputConditionIdentifier

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.4+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
let kCGPDFXOutputConditionIdentifier: CFString
```

## Discussion

A string identifying the intended output device or production condition in a human- or machine-readable form. This key is required. The value of this key must be a CFString object. For best results, the string should be restricted to characters in the ASCII character set.

## See Also

### Output Intent Keys

let kCGPDFXOutputIntentSubtype: CFString

The output intent subtype. This key is required.

let kCGPDFXOutputCondition: CFString

A text string identifying the intended output device or production condition in a human-readable form.

let kCGPDFXRegistryName: CFString

let kCGPDFXInfo: CFString

let kCGPDFXDestinationOutputProfile: CFString

