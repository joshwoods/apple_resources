

- HomeKit
-  HMAccessoryProfile 

Class

# HMAccessoryProfile

A profile that certain accessories implement.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class HMAccessoryProfile
```

## Overview

This is an abstract superclass for classes such as HMCameraProfile and HMNetworkConfigurationProfile. Each profile subclass controls specific features for a specific set of accessories.

## Topics

### Getting information about a profile

var accessory: HMAccessory?

The accessory that implements this profile.

var services: [HMService]

An array of services that represents this profile.

var uniqueIdentifier: UUID

A unique identifier for the profile.

## Relationships

### Inherits From

- NSObject

### Inherited By

- HMCameraProfile
- HMMediaSourceDisplayOrderProfile
- HMNetworkConfigurationProfile

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Managing accessory profiles

var profiles: [HMAccessoryProfile]

An array of profiles implemented by the accessory.

class HMNetworkConfigurationProfile

A profile that provides information about network protection for an accessory.

class HMCameraProfile

A camera profile that interacts with an accessory’s camera.

