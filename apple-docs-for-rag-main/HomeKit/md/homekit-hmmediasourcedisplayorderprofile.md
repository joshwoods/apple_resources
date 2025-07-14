

- HomeKit
-  HMMediaSourceDisplayOrderProfile 

Class

# HMMediaSourceDisplayOrderProfile

An interface from which to read and, if allowed by the accessory, update the ordering of input sources.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
@objc
class HMMediaSourceDisplayOrderProfile
```

## Overview

This class represents a media source display that orders functionality for the HMServiceTypeTelevision service contained in the services array of the profile.

## Topics

### Managing input source order

func writeOrder([Int]) async throws

Writes the display order of the media sources to the accessory.

var delegate: (any HMMediaSourceDisplayOrderProfile.Delegate)?

The property that handles updates to the display order.

var order: [Int]

The display order of input media sources.

let canModifyOrder: Bool

A Boolean that indicates if the display order of the input media sources can be modified.

protocol Delegate

The protocol through which a delegate receives updates on the order of input media sources.

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

### Accessories

class HMAccessorySetupManager

An object that setups up new accessories.

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

