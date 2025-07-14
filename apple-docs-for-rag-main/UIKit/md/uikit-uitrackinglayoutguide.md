

- UIKit
-  UITrackingLayoutGuide 

Class

# UITrackingLayoutGuide

A layout guide that automatically activates and deactivates layout constraints depending on its proximity to edges.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
@MainActor
class UITrackingLayoutGuide
```

## Topics

### Configuring automatic constraint activation

func setConstraints([NSLayoutConstraint], activeWhenNearEdge: NSDirectionalRectEdge)

Configures the tracking layout guide to automatically activate and deactivate constraints when the guide is close to the given edge.

func setConstraints([NSLayoutConstraint], activeWhenAwayFrom: NSDirectionalRectEdge)

Configures the tracking layout guide to automatically activate and deactivate constraints when the guide is away from the given edge.

func constraints(activeWhenNearEdge: NSDirectionalRectEdge) -> [NSLayoutConstraint]

Returns the constraints that the tracking layout guide activates when it’s near the given edge, and deactivates when it’s away from the given edge.

func constraints(activeWhenAwayFrom: NSDirectionalRectEdge) -> [NSLayoutConstraint]

Returns the constraints that the tracking layout guide activates when it’s away from the given edge, and deactivates when it’s near the edge.

### Tracking constraints

func removeAllTrackedConstraints()

Stops the layout guide from tracking any constraints.

## Relationships

### Inherits From

- UILayoutGuide

### Inherited By

- UIKeyboardLayoutGuide

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- Sendable
- UIPopoverPresentationControllerSourceItem

## See Also

### Keyboard layout

Adjusting your layout with keyboard layout guide

Respond dynamically to keyboard movement by using the tracking features of the keyboard layout guide.

class UIKeyboardLayoutGuide

A layout guide that represents the space the keyboard occupies in your app’s layout.

