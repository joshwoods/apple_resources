

- DockKit
- DockAccessory
-  DockAccessory.BatteryChargeState 

Enumeration

# DockAccessory.BatteryChargeState

The charging state of an accessory battery

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+

``` source
enum BatteryChargeState
```

## Topics

### Operators

static func == (DockAccessory.BatteryChargeState, DockAccessory.BatteryChargeState) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case charging

The battery is charging.

case notChargeable

The battery is not a chargeable battery.

case notCharging

The battery is not charging.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

