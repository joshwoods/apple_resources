

- WatchKit
-  WKWaterResistanceRating 

Enumeration

# WKWaterResistanceRating

Values indicating the water-resistance rating.

watchOS 3.0+

``` source
enum WKWaterResistanceRating
```

## Topics

### Enumeration Cases

case ipx7

A water-resistance rating of IPX7.

case wr50

A water-resistance rating of 50 meters.

case wr100

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Accessing Water Resistance and Lock

var waterResistanceRating: WKWaterResistanceRating

The Apple Watch water-resistance rating.

var isWaterLockEnabled: Bool

A Boolean value that indicates whether the water lock is enabled.

func enableWaterLock()

Disables the Apple Watch touch screen to prevent accidental taps while submerged.

