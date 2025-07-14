

- HomeKit
-  HMNetworkConfigurationProfile 

Class

# HMNetworkConfigurationProfile

A profile that provides information about network protection for an accessory.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class HMNetworkConfigurationProfile
```

## Overview

To increase security, HomeKit can restrict network access for specific accessories, including access to other accessories in the home, and to the internet. However, an accessory your app controls might need network access to carry out certain functions, like downloading new firmware.

Check the isNetworkAccessRestricted property of an accessory’s network configuration profile to find out if an accessory has restricted access. You can use this information to ask the user to relax network restrictions in the Home app.

## Topics

### Restricting network access

var isNetworkAccessRestricted: Bool

An indication of whether the accessory’s access to the network is restricted.

### Listening for access changes

var delegate: (any HMNetworkConfigurationProfileDelegate)?

A delegate that HomeKit tells about changes in the state of network access.

protocol HMNetworkConfigurationProfileDelegate

An interface that your app adopts to receive notifications about changes in the state of network access.

## Relationships

### Inherits From

- HMAccessoryProfile

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

class HMAccessoryProfile

A profile that certain accessories implement.

class HMCameraProfile

A camera profile that interacts with an accessory’s camera.

