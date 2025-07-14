

- HomeKit
-  HMService 

Class

# HMService

A controllable feature of an accessory, like a light attached to a garage door opener.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
class HMService
```

## Overview

An HMService instance represents a service provided by an accessory. Accessories have both user-controllable services, like a light, and services that are for the use of the accessory itself, like a firmware update service.

You don’t create services directly. Instead you find them in the services array of an HMAccessory instance.

A single accessory may have more than one user-controllable service. For example, most garage door openers have a service for opening and closing the door, and another service for the light on the garage door opener. These services are what Apple’s Home app labels as “accessories”.

You inspect or change a service’s HMCharacteristic instances to discover state, or modify behavior.

## Topics

### Getting service characteristics

var characteristics: [HMCharacteristic]

An array of characteristics for the service.

class HMCharacteristic

A specific characteristic of a service, like the brightness of a dimmable light or its color temperature.

### Identifying the service

var name: String

The user specified name of the service.

func updateName(String, completionHandler: ((any Error)?) -> Void)

Updates the name of the service to the specified string.

var uniqueIdentifier: UUID

A unique identifier for the service.

### Getting the service type

var serviceType: String

The type of the service.

Accessory Service Types

The service types supported by HomeKit.

var localizedDescription: String

The localized description of the service.

### Reading service properties

var isPrimaryService: Bool

A Boolean value that indicates whether this service is the primary service on the accessory.

var isUserInteractive: Bool

A Boolean value that indicates whether this service supports user interaction.

### Associating a secondary service

var associatedServiceType: String?

The type of the service associated with an outlet or a switch.

func updateAssociatedServiceType(String?, completionHandler: ((any Error)?) -> Void)

Associates the service type of the plugged-in device with a switch or an outlet service.

### Finding the linked services

var linkedServices: [HMService]?

An array of service objects that represents all the services to which the service links.

### Getting the service’s provider

var accessory: HMAccessory?

The accessory that provides this service.

### Initializers

init()Deprecated

### Instance Properties

var matterEndpointID: UInt16?

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

class HMCharacteristic

A specific characteristic of a service, like the brightness of a dimmable light or its color temperature.

class HMMediaSourceDisplayOrderProfile

An interface from which to read and, if allowed by the accessory, update the ordering of input sources.

