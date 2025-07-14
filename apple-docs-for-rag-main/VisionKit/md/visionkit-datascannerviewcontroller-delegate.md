

- VisionKit
- DataScannerViewController
-  delegate 

Instance Property

# delegate

The delegate that handles user interaction with items recognized by the data scanner.

iOS 16.0+iPadOS 16.0+visionOS 1.0+

``` source
@MainActor
weak var delegate: (any DataScannerViewControllerDelegate)?
```

## See Also

### Configuring data scanners

let qualityLevel: DataScannerViewController.QualityLevel

The resolution that the scanner uses to find data.

enum QualityLevel

The possible quality levels that the scanner uses to find data.

let recognizesMultipleItems: Bool

A Boolean value that indicates whether the scanner should identify all items in the live video.

let isHighFrameRateTrackingEnabled: Bool

A Boolean value that determines the frequency at which the scanner updates the geometry of recognized items.

let isPinchToZoomEnabled: Bool

A Boolean value that indicates whether people can use a two-finger pinch-to-zoom gesture.

let isGuidanceEnabled: Bool

A Boolean value that indicates whether the scanner provides help to a person when selecting items.

let isHighlightingEnabled: Bool

A Boolean value that indicates whether the scanner displays highlights around recognized items.

