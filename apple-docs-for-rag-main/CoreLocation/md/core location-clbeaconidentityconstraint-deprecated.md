

- Core Location
-  CLBeaconIdentityConstraint Deprecated

Class

# CLBeaconIdentityConstraint

Identity characteristics that can match one or more beacons.

iOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.15–11.0Deprecated

``` source
class CLBeaconIdentityConstraint
```

Deprecated

Use CLBeaconIdentityCondition instead.

## Overview

A constraint specifies beacon identity characteristics. Use constraints to check for matching beacons by comparing the beacon’s identity characteristics (uuid, major, and minor) to those in the constraint.

Constraints always specify a UUID value, but the major and minor values are optional. A beacon satisfies the constraint if all three identity characteristics of the beacon match the same characteristic of the constraint. Major and minor characteristics are wildcards if they have no value. A major or minor wildcard value matches any value in the beacon’s corresponding characteristic.

## Topics

### Getting the beacon identity

var major: UInt16?

The constraint’s value for the major identity characteristic.

var minor: UInt16?

The constraint’s value for the minor identity characteristic.

## Relationships

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
- Sendable

## See Also

### Classes

class CLBeaconRegion

A region for detecting the presence of iBeacon devices.

Deprecated

class CLCircularRegion

A circular geographic region that a center point and radius deine.

Deprecated

