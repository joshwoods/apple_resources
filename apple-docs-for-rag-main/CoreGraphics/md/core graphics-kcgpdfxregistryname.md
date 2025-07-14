

- Core Graphics
-  kCGPDFXRegistryName 

Global Variable

# kCGPDFXRegistryName

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.4+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
let kCGPDFXRegistryName: CFString
```

## Discussion

A string identifying the registry in which the condition designated by kCGPDFXOutputConditionIdentifier is defined. This key is optional. If present, the value of this key must be a CFString object. For best results, the string should be lossless in ASCII encoding.

## See Also

### Output Intent Keys

let kCGPDFXOutputIntentSubtype: CFString

The output intent subtype. This key is required.

let kCGPDFXOutputConditionIdentifier: CFString

let kCGPDFXOutputCondition: CFString

A text string identifying the intended output device or production condition in a human-readable form.

let kCGPDFXInfo: CFString

let kCGPDFXDestinationOutputProfile: CFString

