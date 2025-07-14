

- AppKit
- NSView
-  removeTrackingRect(\_:) 

Instance Method

# removeTrackingRect(\_:)

Removes the tracking rectangle identified by a tag.

macOS

``` source
@MainActor
func removeTrackingRect(_ tag: NSView.TrackingRectTag)
```

## Parameters 

`tag`  

An integer value identifying a tracking rectangle. It was returned by a previously sent addTrackingRect(_:owner:userData:assumeInside:) message.

## See Also

### Related Documentation

func removeTrackingArea(NSTrackingArea)

Removes a given tracking area from the view.

### Managing Tracking Rectangles

func addTrackingRect(NSRect, owner: Any, userData: UnsafeMutableRawPointer?, assumeInside: Bool) -> NSView.TrackingRectTag

Establishes an area for tracking mouse-entered and mouse-exited events within the view and returns a tag that identifies the tracking rectangle.

typealias TrackingRectTag

This type describes the rectangle used to track the mouse.

