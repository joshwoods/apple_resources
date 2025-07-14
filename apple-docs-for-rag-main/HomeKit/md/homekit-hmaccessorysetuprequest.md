

- HomeKit
-  HMAccessorySetupRequest 

Class

# HMAccessorySetupRequest

An object that describes how to add and setup up new accessories.

iOS 15.4+iPadOS 15.4+

``` source
class HMAccessorySetupRequest
```

## Overview

Use this class to provide steps for the user to add one or more accessories to a particular home, and follow up with additional setup.

## Topics

### Setting up accessorices

var homeUniqueIdentifier: UUID?

The identifier corresponding to the home that the accessory should be added to when being set up.

var payload: HMAccessorySetupPayload?

The payload to use for accessory setup.

var suggestedAccessoryName: String?

The name that the framework suggests when the user names the accessory being set up.

var suggestedRoomUniqueIdentifier: UUID?

The identifier corresponding to the room that the framework suggests.

### Instance Properties

var matterPayload: MTRSetupPayload?

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
- NSCopying
- NSObjectProtocol
- Sendable

## See Also

### Accessories

class HMAccessorySetupManager

An object that setups up new accessories.

class HMAccessorySetupResult

A result object describing information about a successful accessory setup request.

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

