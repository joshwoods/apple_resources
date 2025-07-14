

- Vision
- GeneratePersonSegmentationRequest
-  supportedOutputPixelFormats 

Instance Property

# supportedOutputPixelFormats

The collection of supported pixel format types.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
final var supportedOutputPixelFormats: [OSType] { get }
```

## See Also

### Inspecting a request

var qualityLevel: GeneratePersonSegmentationRequest.QualityLevel

A value that indicates how the request balances accuracy and performance.

enum QualityLevel

Constants that define the levels of quality for a person-segmentation request.

var outputPixelFormatType: OSType

The desired pixel format of the observation.

