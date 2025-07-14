

- UIKit
- UITrackingLayoutGuide
-  constraints(activeWhenNearEdge:) 

Instance Method

# constraints(activeWhenNearEdge:)

Returns the constraints that the tracking layout guide activates when it’s near the given edge, and deactivates when it’s away from the given edge.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
@MainActor
func constraints(activeWhenNearEdge edge: NSDirectionalRectEdge) -> [NSLayoutConstraint]
```

## Parameters 

`edge`  

The edge that the tracking layout guide uses to determine when to activate or deactivate the constraints.

## Return Value

An array of layout constraints that the tracking layout guide automatically activates and deactivates.

## See Also

### Configuring automatic constraint activation

func setConstraints([NSLayoutConstraint], activeWhenNearEdge: NSDirectionalRectEdge)

Configures the tracking layout guide to automatically activate and deactivate constraints when the guide is close to the given edge.

func setConstraints([NSLayoutConstraint], activeWhenAwayFrom: NSDirectionalRectEdge)

Configures the tracking layout guide to automatically activate and deactivate constraints when the guide is away from the given edge.

func constraints(activeWhenAwayFrom: NSDirectionalRectEdge) -> [NSLayoutConstraint]

Returns the constraints that the tracking layout guide activates when it’s away from the given edge, and deactivates when it’s near the edge.

