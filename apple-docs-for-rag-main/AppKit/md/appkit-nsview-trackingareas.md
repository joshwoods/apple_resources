

- AppKit
- NSView
-  trackingAreas 

Instance Property

# trackingAreas

An array of the view’s tracking areas.

macOS 10.5+

``` source
@MainActor
var trackingAreas: [NSTrackingArea] { get }
```

## Discussion

This property contains an array of NSTrackingArea objects. If the view has no tracking areas, the array is empty.

## See Also

### Managing Tracking Areas

func addTrackingArea(NSTrackingArea)

Adds a given tracking area to the view.

func removeTrackingArea(NSTrackingArea)

Removes a given tracking area from the view.

func updateTrackingAreas()

Invoked automatically when the view’s geometry changes such that its tracking areas need to be recalculated.

class let didUpdateTrackingAreasNotification: NSNotification.Name

Posted whenever a view recalculates its tracking areas.

