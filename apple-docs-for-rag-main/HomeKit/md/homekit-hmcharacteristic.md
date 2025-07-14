

- HomeKit
-  HMCharacteristic 

Class

# HMCharacteristic

A specific characteristic of a service, like the brightness of a dimmable light or its color temperature.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
class HMCharacteristic
```

## Overview

An HMCharacteristic instance represents an aspect of a service that provides data, or that your app can control.

You don’t create characteristic instances. Instead, an accessory manufacturer incorporates them into a device, which publishes them to you through the characteristics array of an HMService instance.

Characteristics have a properties array that indicates attributes like readability, writability, and user-visibility. They also have a characteristicType property that tells your app what the characteristic controls or describes. Device manufacturers can use one of the standard types, given in Characteristic types, or they can create custom types.

Each characteristic has a value that you can read or write. Some characteristics use plain numbers, Booleans, or strings. Others have application specific meanings declared in enumerations associated with the given characteristic type. The characteristic’s metadata can help your app interpret the value.

## Topics

### Identifying a characteristic

var uniqueIdentifier: UUID

A unique identifier for the characteristic.

var localizedDescription: String

The localized description of the characteristic.

### Reading characteristic properties

var properties: [String]

An array of properties that describe the characteristic.

Characteristic Properties

The properties that characteristics can have.

### Determining what a characteristic controls

var characteristicType: String

The type of the characteristic.

Characteristic types

The characteristic types supported by HomeKit-based accessories.

### Controlling a characteristic

var value: Any?

The current value of the characteristic.

func readValue(completionHandler: ((any Error)?) -> Void)

Reads the value for the characteristic.

func writeValue(Any?, completionHandler: ((any Error)?) -> Void)

Modifies the value of the characteristic.

func updateAuthorizationData(Data?, completionHandler: ((any Error)?) -> Void)

Sets or clears authorization data used when writing to the characteristic.

### Managing characteristic presentation

var metadata: HMCharacteristicMetadata?

Metadata about the units and other properties of the characteristic.

class HMCharacteristicMetadata

Metadata that describes a characteristic’s value and that may be useful for presentation purposes.

### Receiving change notifications

func enableNotification(Bool, completionHandler: ((any Error)?) -> Void)

Enables or disables notifications for changes in the value of the characteristic.

var isNotificationEnabled: Bool

A Boolean indicating whether the characteristic has been set to send notifications.

### Getting the characterized service

var service: HMService?

The service that contains this characteristic.

### Initializers

init()Deprecated

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

class HMService

A controllable feature of an accessory, like a light attached to a garage door opener.

class HMMediaSourceDisplayOrderProfile

An interface from which to read and, if allowed by the accessory, update the ordering of input sources.

