

- AppKit
- NSView
-  didUpdateTrackingAreasNotification 

Type Property

# didUpdateTrackingAreasNotification

Posted whenever a view recalculates its tracking areas.

macOS 10.5+

``` source
class let didUpdateTrackingAreasNotification: NSNotification.Name
```

## Discussion

It is sent after the view receives updateTrackingAreas().

## See Also

### Managing Tracking Areas

func addTrackingArea(NSTrackingArea)

Adds a given tracking area to the view.

func removeTrackingArea(NSTrackingArea)

Removes a given tracking area from the view.

var trackingAreas: [NSTrackingArea]

An array of the view’s tracking areas.

func updateTrackingAreas()

Invoked automatically when the view’s geometry changes such that its tracking areas need to be recalculated.

