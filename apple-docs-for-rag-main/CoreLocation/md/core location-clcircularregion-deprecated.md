

- Core Location
-  CLCircularRegion Deprecated

Class

# CLCircularRegion

A circular geographic region that a center point and radius deine.

iOS 7.0–18.4DeprecatediPadOS 7.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.10–11.0DeprecatedtvOS 9.0+watchOS 2.0–9.0Deprecated

``` source
class CLCircularRegion
```

Deprecated

Use CLCircularGeographicCondition instead.

## Overview

The CLCircularRegion class defines the location and boundaries for a circular geographic region. You can use instances of this class to define geofences for a specific location. The crossing of a geofence’s boundary causes the location manager to notify its delegate.

## Topics

### Creating a circular region

init(center: CLLocationCoordinate2D, radius: CLLocationDistance, identifier: String)

Creates and returns a region object defining a circular geographic area.

### Getting the circle’s center and radius

var center: CLLocationCoordinate2D

The center point of the geographic area.

var radius: CLLocationDistance

The radius (measured in meters) that defines the geographic area’s outer boundary.

### Performing hit testing in the region

func contains(CLLocationCoordinate2D) -> Bool

Returns a Boolean value indicating whether the geographic area contains the specified coordinate.

## Relationships

### Inherits From

- CLRegion

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Classes

class CLBeaconRegion

A region for detecting the presence of iBeacon devices.

Deprecated

class CLBeaconIdentityConstraint

Identity characteristics that can match one or more beacons.

Deprecated

