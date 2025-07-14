

- UIKit
- UIUpdateInfo
-  modelTime 

Instance Property

# modelTime

The time interval that represents a reference point for the current time of the UI update.

iOS 18.0+iPadOS 18.0+tvOS 18.0+visionOS 2.0+

``` source
@MainActor
var modelTime: TimeInterval { get }
```

## Discussion

This time provides a reference point for driving time-based model changes, like animations or physics. This property attempts to maintain constant latency between model changes and their onscreen presentation. It uses the same units as CACurrentMediaTime(). Numerically, this time is close to the start of the UI update, but its precise relation to the UI update start time might change, depending on frame rate and other UI update parameters.

## See Also

### Getting information about timing

var completionDeadlineTime: TimeInterval

The time interval that represents the time by which an app needs to finish submitting changes to the render server.

var estimatedPresentationTime: TimeInterval

The time interval that represents an estimate for when current UI update changes become visible onscreen.

