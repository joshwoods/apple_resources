

- WatchKit
- WKExtension
-  isAutorotating 

Instance Property

# isAutorotating

A Boolean value that determines whether the interface automatically rotates when the user flips their wrist.

watchOS 4.0+

``` source
@MainActor
var isAutorotating: Bool { get set }
```

## Discussion

Defaults to false.

Normally, when a user rotates their wrist–for example, to show a watchOS app to another person–the watch is likely to interpret this motion as dropping the wrist and may put the app to sleep. When autorotation is enabled, watchOS instead keeps the interface awake and rotates the content so that it is oriented properly for the viewer.

Do not enable autorotation indefinitely. Instead, enable it selectively on a specific interface controller that the user is likely to share. For example, in the interface controller’s willActivate() method, set this property to true. In the didDeactivate() method, set it back to false.

## See Also

### Related Documentation

func deviceOrientationDidChange()

Tells the delegate that the device’s orientation has changed.

### Managing the user interface

var isAutorotated: Bool

A Boolean value that indicates whether the system has automatically rotated the user interface so that it is properly oriented for another viewer.

var globalTintColor: UIColor

The watchOS app’s global tint color.

func enableWaterLock()

Disables the Apple Watch touch screen to prevent accidental taps while the watch is underwater.

Deprecated

