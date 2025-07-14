

- UIKit
- UITrackingLayoutGuide
-  setConstraints(\_:activeWhenNearEdge:) 

Instance Method

# setConstraints(\_:activeWhenNearEdge:)

Configures the tracking layout guide to automatically activate and deactivate constraints when the guide is close to the given edge.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
@MainActor
func setConstraints(
    _ trackingConstraints: [NSLayoutConstraint],
    activeWhenNearEdge edge: NSDirectionalRectEdge
)
```

## Parameters 

`trackingConstraints`  

The constraints to activate when the tracking layout guide is close to `edge`, and to deactivate when it moves away from `edge`. If you pass `nil`, the guide stops tracking the constraints associated with `edge`.

`edge`  

The edge that the tracking layout guide uses to determine whether to activate or deactivate the constraints.

## See Also

### Configuring automatic constraint activation

func setConstraints([NSLayoutConstraint], activeWhenAwayFrom: NSDirectionalRectEdge)

Configures the tracking layout guide to automatically activate and deactivate constraints when the guide is away from the given edge.

func constraints(activeWhenNearEdge: NSDirectionalRectEdge) -> [NSLayoutConstraint]

Returns the constraints that the tracking layout guide activates when it’s near the given edge, and deactivates when it’s away from the given edge.

func constraints(activeWhenAwayFrom: NSDirectionalRectEdge) -> [NSLayoutConstraint]

Returns the constraints that the tracking layout guide activates when it’s away from the given edge, and deactivates when it’s near the edge.

