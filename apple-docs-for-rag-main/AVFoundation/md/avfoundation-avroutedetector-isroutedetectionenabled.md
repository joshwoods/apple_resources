

- AVFoundation
- AVRouteDetector
-  isRouteDetectionEnabled 

Instance Property

# isRouteDetectionEnabled

A Boolean value that indicates whether route detection is in an enabled state.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var isRouteDetectionEnabled: Bool { get set }
```

## Discussion

The default value is false.

Note

Enabling route detection significantly increases power consumption. Turn it off when you no longer need it.

## See Also

### Detecting Routes

var detectsCustomRoutes: Bool

A Boolean value that indicates whether route detection includes custom routes.

var multipleRoutesDetected: Bool

A Boolean value that indicates whether the object detects more than one playback route.

static let AVRouteDetectorMultipleRoutesDetectedDidChange: NSNotification.Name

A notification the system posts when changes occur to its detected routes.

