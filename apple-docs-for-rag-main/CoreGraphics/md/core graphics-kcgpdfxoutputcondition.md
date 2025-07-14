

- Core Graphics
-  kCGPDFXOutputCondition 

Global Variable

# kCGPDFXOutputCondition

A text string identifying the intended output device or production condition in a human-readable form.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.4+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
let kCGPDFXOutputCondition: CFString
```

## Discussion

This key is optional. If present, the value of this key must be a CFString object.

## See Also

### Output Intent Keys

let kCGPDFXOutputIntentSubtype: CFString

The output intent subtype. This key is required.

let kCGPDFXOutputConditionIdentifier: CFString

let kCGPDFXRegistryName: CFString

let kCGPDFXInfo: CFString

let kCGPDFXDestinationOutputProfile: CFString

