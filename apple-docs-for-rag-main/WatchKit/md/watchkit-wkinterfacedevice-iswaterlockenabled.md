

- WatchKit
- WKInterfaceDevice
-  isWaterLockEnabled 

Instance Property

# isWaterLockEnabled

A Boolean value that indicates whether the water lock is enabled.

watchOS 6.1+

``` source
var isWaterLockEnabled: Bool { get }
```

## See Also

### Accessing Water Resistance and Lock

var waterResistanceRating: WKWaterResistanceRating

The Apple Watch water-resistance rating.

enum WKWaterResistanceRating

Values indicating the water-resistance rating.

func enableWaterLock()

Disables the Apple Watch touch screen to prevent accidental taps while submerged.

