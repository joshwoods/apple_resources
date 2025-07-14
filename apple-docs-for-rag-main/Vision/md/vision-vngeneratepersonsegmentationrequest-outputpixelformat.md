

- Vision
- VNGeneratePersonSegmentationRequest
-  outputPixelFormat 

Instance Property

# outputPixelFormat

The pixel format of the output image.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
var outputPixelFormat: OSType { get set }
```

## Discussion

The property supports the following values:

- kCVPixelFormatType_OneComponent8

- kCVPixelFormatType_OneComponent16Half

- kCVPixelFormatType_OneComponent32Float

The default value is kCVPixelFormatType_OneComponent8.

## See Also

### Configuring the Request

var qualityLevel: VNGeneratePersonSegmentationRequest.QualityLevel

A value that indicates how the request balances accuracy and performance.

enum QualityLevel

Constants that define the levels of quality for a person segmentation request.

