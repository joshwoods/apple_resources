

- WatchKit
- WKInterfaceDevice
-  waterResistanceRating 

Instance Property

# waterResistanceRating

The Apple Watch water-resistance rating.

watchOS 3.0+

``` source
var waterResistanceRating: WKWaterResistanceRating { get }
```

## Discussion

For a list of possible water resistance ratings, see WKWaterResistanceRating.

## See Also

### Accessing Water Resistance and Lock

enum WKWaterResistanceRating

Values indicating the water-resistance rating.

var isWaterLockEnabled: Bool

A Boolean value that indicates whether the water lock is enabled.

func enableWaterLock()

Disables the Apple Watch touch screen to prevent accidental taps while submerged.

