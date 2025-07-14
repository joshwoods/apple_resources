

- VisionKit
- DataScannerViewController
-  isGuidanceEnabled 

Instance Property

# isGuidanceEnabled

A Boolean value that indicates whether the scanner provides help to a person when selecting items.

iOS 16.0+iPadOS 16.0+visionOS 1.0+

``` source
@MainActor
final let isGuidanceEnabled: Bool
```

## Discussion

The guidance text, such as “Slow Down,” appears over the live video. The default value for this property is `true`.

## See Also

### Configuring data scanners

var delegate: (any DataScannerViewControllerDelegate)?

The delegate that handles user interaction with items recognized by the data scanner.

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

let isHighlightingEnabled: Bool

A Boolean value that indicates whether the scanner displays highlights around recognized items.

