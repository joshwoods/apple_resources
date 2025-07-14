

- AVFoundation
- AVRouteDetector
-  detectsCustomRoutes 

Instance Property

# detectsCustomRoutes

A Boolean value that indicates whether route detection includes custom routes.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
var detectsCustomRoutes: Bool { get set }
```

## Discussion

The default value is false. Only set it to true if your app uses an instance of AVCustomRoutingController.

## See Also

### Detecting Routes

var isRouteDetectionEnabled: Bool

A Boolean value that indicates whether route detection is in an enabled state.

var multipleRoutesDetected: Bool

A Boolean value that indicates whether the object detects more than one playback route.

static let AVRouteDetectorMultipleRoutesDetectedDidChange: NSNotification.Name

A notification the system posts when changes occur to its detected routes.

