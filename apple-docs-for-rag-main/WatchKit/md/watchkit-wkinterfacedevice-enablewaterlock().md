

- WatchKit
- WKInterfaceDevice
-  enableWaterLock() 

Instance Method

# enableWaterLock()

Disables the Apple Watch touch screen to prevent accidental taps while submerged.

watchOS 6.1+

``` source
func enableWaterLock()
```

## Discussion

The following rules apply when using Water Lock:

- You must call the enableWaterLock() method from the main thread.

- You can only enable Water Lock when the app is running in the foreground during an active workout or location session.

- The app must be running on a supported device (the WKInterfaceDevice object’s waterResistanceRating property must be WKWaterResistanceRating.wr50).

- Water Lock remains active until the user unlocks it. You can’t programmatically unlock the watch.

## See Also

### Accessing Water Resistance and Lock

var waterResistanceRating: WKWaterResistanceRating

The Apple Watch water-resistance rating.

enum WKWaterResistanceRating

Values indicating the water-resistance rating.

var isWaterLockEnabled: Bool

A Boolean value that indicates whether the water lock is enabled.

