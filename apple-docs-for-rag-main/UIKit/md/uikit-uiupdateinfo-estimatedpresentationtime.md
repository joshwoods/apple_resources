

- UIKit
- UIUpdateInfo
-  estimatedPresentationTime 

Instance Property

# estimatedPresentationTime

The time interval that represents an estimate for when current UI update changes become visible onscreen.

iOS 18.0+iPadOS 18.0+tvOS 18.0+visionOS 2.0+

``` source
@MainActor
var estimatedPresentationTime: TimeInterval { get }
```

## Discussion

This time is an estimate, so the actual time when changes become visible might differ.

## See Also

### Getting information about timing

var modelTime: TimeInterval

The time interval that represents a reference point for the current time of the UI update.

var completionDeadlineTime: TimeInterval

The time interval that represents the time by which an app needs to finish submitting changes to the render server.

