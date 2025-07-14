

- Core Location
-  CLProximity 

Enumeration

# CLProximity

Constants that reflect the relative distance to a beacon.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.15+

``` source
enum CLProximity
```

## Topics

### Proximity Values

case unknown

The proximity of the beacon could not be determined.

case immediate

The beacon is in the user’s immediate vicinity.

case near

The beacon is relatively close to the user.

case far

The beacon is far away.

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

### Determining the distance to the beacon

var proximity: CLProximity

The relative distance to the beacon.

var accuracy: CLLocationAccuracy

The accuracy of the proximity value, measured in meters from the beacon.

var rssi: Int

The received signal strength of the beacon, measured in decibels.

