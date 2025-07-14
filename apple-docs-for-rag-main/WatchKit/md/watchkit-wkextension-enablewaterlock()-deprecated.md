

- WatchKit
- WKExtension
-  enableWaterLock() Deprecated

Instance Method

# enableWaterLock()

Disables the Apple Watch touch screen to prevent accidental taps while the watch is underwater.

watchOS 4.0–6.1Deprecated

``` source
@MainActor
func enableWaterLock()
```

Deprecated

Use the WKInterfaceDevice class’s enableWaterLock() method instead.

## Discussion

The following rules apply when using Water Lock:

- You must call the enableWaterLock() method from the main thread.

- You can only enable Water Lock when the app is running in the foreground during an active workout or location session.

- The app must be running on a supported device (the WKInterfaceDevice object’s waterResistanceRating property must be set to WKWaterResistanceRating.wr50).

- Water Lock remains active until the user unlocks it. You can’t programmatically unlock the watch.

## See Also

### Managing the user interface

var isAutorotating: Bool

A Boolean value that determines whether the interface automatically rotates when the user flips their wrist.

var isAutorotated: Bool

A Boolean value that indicates whether the system has automatically rotated the user interface so that it is properly oriented for another viewer.

var globalTintColor: UIColor

The watchOS app’s global tint color.

