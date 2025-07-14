

- AppKit
- NSView
-  NSView.TrackingRectTag 

Type Alias

# NSView.TrackingRectTag

This type describes the rectangle used to track the mouse.

macOS

``` source
typealias TrackingRectTag = Int
```

## Discussion

If the value of this type is 0, it is invalid. See the methods addTrackingRect(_:owner:userData:assumeInside:) and removeTrackingRect(_:).

## See Also

### Managing Tracking Rectangles

func addTrackingRect(NSRect, owner: Any, userData: UnsafeMutableRawPointer?, assumeInside: Bool) -> NSView.TrackingRectTag

Establishes an area for tracking mouse-entered and mouse-exited events within the view and returns a tag that identifies the tracking rectangle.

func removeTrackingRect(NSView.TrackingRectTag)

Removes the tracking rectangle identified by a tag.

