

- AppKit
- NSView
-  removeTrackingArea(\_:) 

Instance Method

# removeTrackingArea(\_:)

Removes a given tracking area from the view.

macOS 10.5+

``` source
@MainActor
func removeTrackingArea(_ trackingArea: NSTrackingArea)
```

## Parameters 

`trackingArea`  

The tracking area to remove from the view.

## See Also

### Managing Tracking Areas

func addTrackingArea(NSTrackingArea)

Adds a given tracking area to the view.

var trackingAreas: [NSTrackingArea]

An array of the view’s tracking areas.

func updateTrackingAreas()

Invoked automatically when the view’s geometry changes such that its tracking areas need to be recalculated.

class let didUpdateTrackingAreasNotification: NSNotification.Name

Posted whenever a view recalculates its tracking areas.

