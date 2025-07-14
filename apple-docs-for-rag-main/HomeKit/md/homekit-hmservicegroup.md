

- HomeKit
-  HMServiceGroup 

Class

# HMServiceGroup

A collection of accessory services.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
class HMServiceGroup
```

## Overview

A service group makes it easier to address the services as a single entity. For example, a user might choose to group a set of lights together as “Desk Lamps,” and have another set of lights grouped as “Ceiling Lights”. You create service groups using the addServiceGroup(withName:completionHandler:) method of HMHome. Service groups are visible to Siri and allow users to control a group of services through Siri.

## Topics

### Managing Service Groups

var name: String

The name of the service group.

var uniqueIdentifier: UUID

The unique identifier for the service group.

func updateName(String, completionHandler: ((any Error)?) -> Void)

Updates the name of the service group.

var services: [HMService]

Array of the services in the service group.

func addService(HMService, completionHandler: ((any Error)?) -> Void)

Adds a new service to the service group.

func removeService(HMService, completionHandler: ((any Error)?) -> Void)

Removes a service from the service group.

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

### Grouping services

func servicesWithTypes([String]) -> [HMService]?

Returns an array of all services provided by accessories in the home that match the specified types.

var serviceGroups: [HMServiceGroup]

An array of all service groups in the home.

func addServiceGroup(withName: String, completionHandler: (HMServiceGroup?, (any Error)?) -> Void)

Adds a service group to the home.

func removeServiceGroup(HMServiceGroup, completionHandler: ((any Error)?) -> Void)

Removes a service group from the home.

