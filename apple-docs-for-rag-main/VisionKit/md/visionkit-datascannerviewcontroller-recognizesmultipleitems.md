

- VisionKit
- DataScannerViewController
-  recognizesMultipleItems 

Instance Property

# recognizesMultipleItems

A Boolean value that indicates whether the scanner should identify all items in the live video.

iOS 16.0+iPadOS 16.0+visionOS 1.0+

``` source
@MainActor
final let recognizesMultipleItems: Bool
```

## Discussion

If `true`, the scanner finds all items in the live video. If `false`, the scanner finds only the item closest to a person’s point of interest. The point of interest is the middle of the view by default or where a person taps in the live video. The default value is `false`.

## See Also

### Configuring data scanners

var delegate: (any DataScannerViewControllerDelegate)?

The delegate that handles user interaction with items recognized by the data scanner.

let qualityLevel: DataScannerViewController.QualityLevel

The resolution that the scanner uses to find data.

enum QualityLevel

The possible quality levels that the scanner uses to find data.

let isHighFrameRateTrackingEnabled: Bool

A Boolean value that determines the frequency at which the scanner updates the geometry of recognized items.

let isPinchToZoomEnabled: Bool

A Boolean value that indicates whether people can use a two-finger pinch-to-zoom gesture.

let isGuidanceEnabled: Bool

A Boolean value that indicates whether the scanner provides help to a person when selecting items.

let isHighlightingEnabled: Bool

A Boolean value that indicates whether the scanner displays highlights around recognized items.

