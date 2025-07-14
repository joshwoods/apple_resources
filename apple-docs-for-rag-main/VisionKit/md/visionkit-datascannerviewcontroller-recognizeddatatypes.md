

- VisionKit
- DataScannerViewController
-  recognizedDataTypes 

Instance Property

# recognizedDataTypes

The types of data that the data scanner identifies in the live video.

iOS 16.0+iPadOS 16.0+visionOS 1.0+

``` source
@MainActor
final let recognizedDataTypes: Set
```

## See Also

### Creating data scanners

init(recognizedDataTypes: Set&lt;DataScannerViewController.RecognizedDataType>, qualityLevel: DataScannerViewController.QualityLevel, recognizesMultipleItems: Bool, isHighFrameRateTrackingEnabled: Bool, isPinchToZoomEnabled: Bool, isGuidanceEnabled: Bool, isHighlightingEnabled: Bool)

Creates a scanner for finding data, such as text and machine-readable codes, in the camera’s live video.

struct RecognizedDataType

A type of data that the scanner recognizes.

