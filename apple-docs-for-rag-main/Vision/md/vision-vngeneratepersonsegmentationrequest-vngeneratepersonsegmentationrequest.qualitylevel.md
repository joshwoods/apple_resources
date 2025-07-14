

- Vision
- VNGeneratePersonSegmentationRequest
-  VNGeneratePersonSegmentationRequest.QualityLevel 

Enumeration

# VNGeneratePersonSegmentationRequest.QualityLevel

Constants that define the levels of quality for a person segmentation request.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
enum QualityLevel
```

## Topics

### Quality Levels

case accurate

Prefers image quality over performance.

case balanced

Prefers processing that balances image quality and performance.

case fast

Prefers performance over image quality.

### Creating a Quality Level

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring the Request

var outputPixelFormat: OSType

The pixel format of the output image.

var qualityLevel: VNGeneratePersonSegmentationRequest.QualityLevel

A value that indicates how the request balances accuracy and performance.

