

- VisionKit
- DataScannerViewController
-  init(recognizedDataTypes:qualityLevel:recognizesMultipleItems:isHighFrameRateTrackingEnabled:isPinchToZoomEnabled:isGuidanceEnabled:isHighlightingEnabled:) 

Initializer

# init(recognizedDataTypes:qualityLevel:recognizesMultipleItems:isHighFrameRateTrackingEnabled:isPinchToZoomEnabled:isGuidanceEnabled:isHighlightingEnabled:)

Creates a scanner for finding data, such as text and machine-readable codes, in the camera’s live video.

iOS 16.0+iPadOS 16.0+visionOS 1.0+

``` source
@MainActor
init(
    recognizedDataTypes: Set,
    qualityLevel: DataScannerViewController.QualityLevel = .balanced,
    recognizesMultipleItems: Bool = false,
    isHighFrameRateTrackingEnabled: Bool = true,
    isPinchToZoomEnabled: Bool = true,
    isGuidanceEnabled: Bool = true,
    isHighlightingEnabled: Bool = false
)
```

## Parameters 

`recognizedDataTypes`  

The types of data that the data scanner identifies in the live video.

`qualityLevel`  

The level of resolution to scan that depends on the size of the items.

`recognizesMultipleItems`  

A Boolean value that indicates whether the scanner identifies all items in the live video.

`isHighFrameRateTrackingEnabled`  

A Boolean value that determines the frequency that the scanner updates the geometry of recognized items.

`isPinchToZoomEnabled`  

A Boolean value that indicates whether people can use a two-finger pinch-to-zoom gesture.

`isGuidanceEnabled`  

A Boolean value that indicates whether the scanner provides help to a person when selecting items.

`isHighlightingEnabled`  

A Boolean value that indicates whether the scanner displays highlights around recognized items.

## See Also

### Related Documentation

let qualityLevel: DataScannerViewController.QualityLevel

The resolution that the scanner uses to find data.

let recognizesMultipleItems: Bool

A Boolean value that indicates whether the scanner should identify all items in the live video.

let isHighFrameRateTrackingEnabled: Bool

A Boolean value that determines the frequency at which the scanner updates the geometry of recognized items.

let isGuidanceEnabled: Bool

A Boolean value that indicates whether the scanner provides help to a person when selecting items.

### Creating data scanners

let recognizedDataTypes: Set&lt;DataScannerViewController.RecognizedDataType>

The types of data that the data scanner identifies in the live video.

struct RecognizedDataType

A type of data that the scanner recognizes.

