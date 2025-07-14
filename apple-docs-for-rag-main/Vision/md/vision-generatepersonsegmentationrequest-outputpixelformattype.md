

- Vision
- GeneratePersonSegmentationRequest
-  outputPixelFormatType 

Instance Property

# outputPixelFormatType

The desired pixel format of the observation.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
final var outputPixelFormatType: OSType { get set }
```

## Discussion

The default value is kCVPixelFormatType_OneComponent8.

## See Also

### Inspecting a request

var qualityLevel: GeneratePersonSegmentationRequest.QualityLevel

A value that indicates how the request balances accuracy and performance.

enum QualityLevel

Constants that define the levels of quality for a person-segmentation request.

var supportedOutputPixelFormats: [OSType]

The collection of supported pixel format types.

