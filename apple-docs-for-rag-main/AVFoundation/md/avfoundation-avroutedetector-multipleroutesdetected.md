

- AVFoundation
- AVRouteDetector
-  multipleRoutesDetected 

Instance Property

# multipleRoutesDetected

A Boolean value that indicates whether the object detects more than one playback route.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var multipleRoutesDetected: Bool { get }
```

## Discussion

The system posts a AVRouteDetectorMultipleRoutesDetectedDidChangeNotification notification when this property value changes.

## See Also

### Detecting Routes

var detectsCustomRoutes: Bool

A Boolean value that indicates whether route detection includes custom routes.

var isRouteDetectionEnabled: Bool

A Boolean value that indicates whether route detection is in an enabled state.

static let AVRouteDetectorMultipleRoutesDetectedDidChange: NSNotification.Name

A notification the system posts when changes occur to its detected routes.

