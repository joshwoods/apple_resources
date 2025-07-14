

- AppKit
- NSView
-  updateTrackingAreas() 

Instance Method

# updateTrackingAreas()

Invoked automatically when the view’s geometry changes such that its tracking areas need to be recalculated.

macOS 10.5+

``` source
@MainActor
func updateTrackingAreas()
```

## Discussion

You should override this method to remove out of date tracking areas and add recomputed tracking areas; your implementation should call `super`.

## See Also

### Managing Tracking Areas

func addTrackingArea(NSTrackingArea)

Adds a given tracking area to the view.

func removeTrackingArea(NSTrackingArea)

Removes a given tracking area from the view.

var trackingAreas: [NSTrackingArea]

An array of the view’s tracking areas.

class let didUpdateTrackingAreasNotification: NSNotification.Name

Posted whenever a view recalculates its tracking areas.

