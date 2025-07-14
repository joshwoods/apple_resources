

- VisionKit
- DataScannerViewController
-  DataScannerViewController.QualityLevel 

Enumeration

# DataScannerViewController.QualityLevel

The possible quality levels that the scanner uses to find data.

iOS 16.0+iPadOS 16.0+visionOS 1.0+

``` source
enum QualityLevel
```

## Overview

The quality levels mostly impact the camera resolution.

## Topics

### Identifying quality levels

case balanced

A quality level that’s between fast and accurate.

case fast

A quality level that prioritizes recognition speed over accuracy.

case accurate

A quality level that prioritizes recognition accuracy over speed.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Configuring data scanners

var delegate: (any DataScannerViewControllerDelegate)?

The delegate that handles user interaction with items recognized by the data scanner.

let qualityLevel: DataScannerViewController.QualityLevel

The resolution that the scanner uses to find data.

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

