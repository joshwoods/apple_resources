

- UIKit
- UIUpdateInfo
-  completionDeadlineTime 

Instance Property

# completionDeadlineTime

The time interval that represents the time by which an app needs to finish submitting changes to the render server.

iOS 18.0+iPadOS 18.0+tvOS 18.0+visionOS 2.0+

``` source
@MainActor
var completionDeadlineTime: TimeInterval { get }
```

## Discussion

Missing this completion deadline results in a presentation delay.

## See Also

### Getting information about timing

var modelTime: TimeInterval

The time interval that represents a reference point for the current time of the UI update.

var estimatedPresentationTime: TimeInterval

The time interval that represents an estimate for when current UI update changes become visible onscreen.

