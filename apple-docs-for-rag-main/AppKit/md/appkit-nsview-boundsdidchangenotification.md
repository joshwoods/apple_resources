

- AppKit
- NSView
-  boundsDidChangeNotification 

Type Property

# boundsDidChangeNotification

Posted whenever the `NSView`‘s bounds rectangle changes to a new value independently of the frame rectangle, but only when the view’s postsBoundsChangedNotifications property is true.

macOS

``` source
class let boundsDidChangeNotification: NSNotification.Name
```

## Discussion

The notification object is the `NSView` object whose bounds rectangle has changed. This notification does not contain a `userInfo` dictionary.

The following methods can result in notification posting:

- bounds

- setBoundsOrigin(_:)

- boundsRotation

- setBoundsSize(_:)

- translateOrigin(to:)

- scaleUnitSquare(to:)

- rotate(byDegrees:)

Note that the bounds rectangle resizes automatically to track the frame rectangle. However, changes to the frame rectangle do not result in this bounds-changed notification.

## See Also

### Modifying the Bounds Rectangle

var bounds: NSRect

The view’s bounds rectangle, which expresses its location and size in its own coordinate system.

func setBoundsOrigin(NSPoint)

Sets the origin of the view’s bounds rectangle to a specified point.

func setBoundsSize(NSSize)

Sets the size of the view’s bounds rectangle to specified dimensions, inversely scaling its coordinate system relative to its frame rectangle.

var boundsRotation: CGFloat

The angle of rotation, measured in degrees, applied to the view’s bounds rectangle relative to its frame rectangle.

var postsBoundsChangedNotifications: Bool

A Boolean value indicating whether the view posts notifications when its bounds rectangle changes.

