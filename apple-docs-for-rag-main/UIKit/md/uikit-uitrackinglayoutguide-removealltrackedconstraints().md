

- UIKit
- UITrackingLayoutGuide
-  removeAllTrackedConstraints() 

Instance Method

# removeAllTrackedConstraints()

Stops the layout guide from tracking any constraints.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
@MainActor
func removeAllTrackedConstraints()
```

## Discussion

This method stops only the tracking of constraints. It doesn’t remove constraints from the layout, and it doesn’t activate or deactivate any constraints.

