

- WatchKit
- WKApplication
-  isAutorotated 

Instance Property

# isAutorotated

A Boolean value that indicates whether the system has automatically rotated the user interface, orienting it properly for another viewer.

watchOS 7.0+

``` source
@MainActor
var isAutorotated: Bool { get }
```

## Discussion

Normally, when a user rotates their wrist–for example, to show a watchOS app to another person–the watch is likely to interpret this motion as dropping the wrist and may put the app to sleep. When you enable autorotation, watchOS instead keeps the interface awake and rotates the content, orienting it properly for the viewer.

For more information on enabling autorotation, see isAutorotating.

## See Also

### Related Documentation

var isAutorotating: Bool

A Boolean value that determines whether the interface automatically rotates when the user flips their wrist.

func deviceOrientationDidChange()

Tells the delegate that the device’s orientation has changed.

### Managing the user interface

var isAutorotating: Bool

A Boolean value that determines whether the interface automatically rotates when the user flips their wrist.

var globalTintColor: UIColor

The watchOS app’s global tint color.

