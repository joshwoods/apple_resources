

- Vision
- GeneratePersonSegmentationRequest
-  GeneratePersonSegmentationRequest.QualityLevel 

Enumeration

# GeneratePersonSegmentationRequest.QualityLevel

Constants that define the levels of quality for a person-segmentation request.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
enum QualityLevel
```

## Topics

### Getting the quality levels

case accurate

A quality option that prefers image quality over performance.

case balanced

A quality option that prefers processing that balances image quality and performance.

case fast

A quality option that prefers performance over image quality.

## Relationships

### Conforms To

- CaseIterable
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Inspecting a request

var qualityLevel: GeneratePersonSegmentationRequest.QualityLevel

A value that indicates how the request balances accuracy and performance.

var outputPixelFormatType: OSType

The desired pixel format of the observation.

var supportedOutputPixelFormats: [OSType]

The collection of supported pixel format types.

