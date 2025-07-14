

- HealthKit
-  HKCharacteristicTypeIdentifier 

Structure

# HKCharacteristicTypeIdentifier

The identifiers that create characteristic type objects.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
struct HKCharacteristicTypeIdentifier
```

## Overview

To create an HKCharacteristicType instance, pass an HKCharacteristicTypeIdentifier value to the characteristicType(forIdentifier:) method.

## Topics

### Characteristic Types

static let activityMoveMode: HKCharacteristicTypeIdentifier

A characteristic identifier for the user’s activity mode.

static let biologicalSex: HKCharacteristicTypeIdentifier

A characteristic type identifier for the user’s sex.

static let bloodType: HKCharacteristicTypeIdentifier

A characteristic type identifier for the user’s blood type.

static let dateOfBirth: HKCharacteristicTypeIdentifier

A characteristic type identifier for the user’s date of birth.

static let fitzpatrickSkinType: HKCharacteristicTypeIdentifier

A characteristic type identifier for the user’s skin type.

static let wheelchairUse: HKCharacteristicTypeIdentifier

A characteristic identifier for the user’s use of a wheelchair.

### Initializers

init(rawValue: String)

Returns a newly initialized characteristic type identifier using the provided string.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Creating characteristic types

class func characteristicType(forIdentifier: HKCharacteristicTypeIdentifier) -> HKCharacteristicType?

Returns the shared characteristic type for the provided identifier.

