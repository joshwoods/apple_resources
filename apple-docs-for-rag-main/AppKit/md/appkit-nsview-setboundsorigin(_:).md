

- AppKit
- NSView
-  setBoundsOrigin(\_:) 

Instance Method

# setBoundsOrigin(\_:)

Sets the origin of the view’s bounds rectangle to a specified point.

macOS

``` source
@MainActor
func setBoundsOrigin(_ newOrigin: NSPoint)
```

## Parameters 

`newOrigin`  

A point specifying the new bounds origin of the view.

## Discussion

In setting the new bounds origin, this method effectively shifts the view’s coordinate system so `newOrigin` lies at the origin of the view’s frame rectangle. It neither redisplays the view nor marks it as needing display. Set the needsDisplay property to true when you want the view to be redisplayed.

This method posts an boundsDidChangeNotification to the default notification center if the view is configured to do so.

After calling this method, `NSView` creates an internal transform (or appends these changes to an existing internal transform) to convert from frame coordinates to bounds coordinates in your view. As long as the width-to-height ratio of the two coordinate systems remains the same, your content appears normal. If the ratios differ, your content may appear skewed.

## See Also

### Related Documentation

func translateOrigin(to: NSPoint)

Translates the view’s coordinate system so that its origin moves to a new location.

### Modifying the Bounds Rectangle

var bounds: NSRect

The view’s bounds rectangle, which expresses its location and size in its own coordinate system.

func setBoundsSize(NSSize)

Sets the size of the view’s bounds rectangle to specified dimensions, inversely scaling its coordinate system relative to its frame rectangle.

var boundsRotation: CGFloat

The angle of rotation, measured in degrees, applied to the view’s bounds rectangle relative to its frame rectangle.

class let boundsDidChangeNotification: NSNotification.Name

Posted whenever the `NSView`‘s bounds rectangle changes to a new value independently of the frame rectangle, but only when the view’s postsBoundsChangedNotifications property is true.

var postsBoundsChangedNotifications: Bool

A Boolean value indicating whether the view posts notifications when its bounds rectangle changes.

