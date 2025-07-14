

- HomeKit
-  HMAccessorySetupManager 

Class

# HMAccessorySetupManager

An object that setups up new accessories.

iOS 15.0+iPadOS 15.0+

``` source
class HMAccessorySetupManager
```

## Overview

Use this class to provides steps for the user to add one or more accessories to a particular home, and follow up with additional setup. These APIs don’t require that the current app has home data authorization.

## Topics

### Adding accessories

func performAccessorySetup(using: HMAccessorySetupRequest, completionHandler: (HMAccessorySetupResult?, (any Error)?) -> Void)

Performs the process of setting up accessories with Apple Home.

### Initializers

init()

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Accessories

class HMAccessorySetupResult

A result object describing information about a successful accessory setup request.

class HMAccessorySetupRequest

An object that describes how to add and setup up new accessories.

Interacting with a home automation network

Find all the automation accessories in the primary home and control their state.

class HMAccessory

A home automation accessory, like a garage door opener or a thermostat.

class HMService

A controllable feature of an accessory, like a light attached to a garage door opener.

class HMCharacteristic

A specific characteristic of a service, like the brightness of a dimmable light or its color temperature.

class HMMediaSourceDisplayOrderProfile

An interface from which to read and, if allowed by the accessory, update the ordering of input sources.

