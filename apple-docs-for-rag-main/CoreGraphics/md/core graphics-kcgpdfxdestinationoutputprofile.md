

- Core Graphics
-  kCGPDFXDestinationOutputProfile 

Global Variable

# kCGPDFXDestinationOutputProfile

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.4+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
let kCGPDFXDestinationOutputProfile: CFString
```

## Discussion

An ICC profile stream defining the transformation from the PDF document’s source colors to output device colorants. This key is required if the value of kCGPDFXOutputConditionIdentifier does not specify a standard production condition. It is optional otherwise. If present, the value of this key must be an ICC-based color space specified as a `CGColorSpace` object.

## See Also

### Output Intent Keys

let kCGPDFXOutputIntentSubtype: CFString

The output intent subtype. This key is required.

let kCGPDFXOutputConditionIdentifier: CFString

let kCGPDFXOutputCondition: CFString

A text string identifying the intended output device or production condition in a human-readable form.

let kCGPDFXRegistryName: CFString

let kCGPDFXInfo: CFString

