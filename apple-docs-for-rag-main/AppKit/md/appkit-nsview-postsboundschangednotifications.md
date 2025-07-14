

- AppKit
- NSView
-  postsBoundsChangedNotifications 

Instance Property

# postsBoundsChangedNotifications

A Boolean value indicating whether the view posts notifications when its bounds rectangle changes.

macOS

``` source
@MainActor
var postsBoundsChangedNotifications: Bool { get set }
```

## Discussion

When the value of this property is true and the view’s bounds rectangle changes to a new value, the view posts a boundsDidChangeNotification to the default notification center. The notification is not posted when you set the bounds rectangle to the value it already has. The default value of this property is true.

If the value of this property is currently false and the bounds have changed, changing the value to true causes the view to post a boundsDidChangeNotification notification immediately. This happens even when there has been no net change in the view’s bounds rectangle.

The following methods and properties can trigger a frame change notification:

- bounds

- setBoundsOrigin(_:)

- setBoundsSize(_:)

- boundsRotation

- translateOrigin(to:)

- scaleUnitSquare(to:)

- rotate(byDegrees:)

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

class let boundsDidChangeNotification: NSNotification.Name

Posted whenever the `NSView`‘s bounds rectangle changes to a new value independently of the frame rectangle, but only when the view’s postsBoundsChangedNotifications property is true.

