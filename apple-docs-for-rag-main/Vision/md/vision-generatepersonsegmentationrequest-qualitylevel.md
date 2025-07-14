

- Vision
- GeneratePersonSegmentationRequest
-  qualityLevel 

Instance Property

# qualityLevel

A value that indicates how the request balances accuracy and performance.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
final var qualityLevel: GeneratePersonSegmentationRequest.QualityLevel { get set }
```

## Discussion

The default is GeneratePersonSegmentationRequest.QualityLevel.accurate.

## See Also

### Inspecting a request

enum QualityLevel

Constants that define the levels of quality for a person-segmentation request.

var outputPixelFormatType: OSType

The desired pixel format of the observation.

var supportedOutputPixelFormats: [OSType]

The collection of supported pixel format types.

