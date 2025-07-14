

- HomeKit
-  HMAccessory 

Class

# HMAccessory

A home automation accessory, like a garage door opener or a thermostat.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
class HMAccessory
```

## Overview

An HMAccessory instance represents a physical device, like a garage door opener, installed in a home and assigned to a room.

You don’t create accessories directly. Instead you get them from the accessories array of an HMHome instance when you want all the accessories in a home, or the accessories array of an HMRoom instance when you want all the accessories in a particular room. Each physical accessory in the home is represented by exactly one accessory instance, so that one instance appears in both a home and a room collection. This is because it’s simultaneously part of the home and in one of the home’s rooms.

When you want to add new accessories, you call the home’s addAndSetupAccessories(completionHandler:) method. In response, HomeKit presents the user with an interface that steps through the process of searching for new accessories in the physical environment, naming them, and assigning them to a room.

Accessories provide one or more services, represented by instances of HMService, that are the features that the user can control, like the light attached to a garage door opener, or the door opener mechanism itself.

## Topics

### Tracking changes to an accessory

var delegate: (any HMAccessoryDelegate)?

A delegate that receives updates on the state of the accessory.

protocol HMAccessoryDelegate

A set of methods that defines the communication method for state updates from accessories to their delegates.

### Identifying an Accessory

var name: String

The name of the accessory.

func updateName(String, completionHandler: ((any Error)?) -> Void)

Changes the name of the accessory.

var uniqueIdentifier: UUID

A unique identifier for the accessory.

var identifier: UUID

A unique identifier for the accessory.

Deprecated

### Categorizing an accessory

var category: HMAccessoryCategory

The category to which the accessory belongs.

class HMAccessoryCategory

A category for a HomeKit accessory.

### Locating an accessory

var room: HMRoom?

The room containing the accessory.

class HMRoom

The smallest subdivision of a home’s space.

### Managing accessory profiles

var profiles: [HMAccessoryProfile]

An array of profiles implemented by the accessory.

class HMAccessoryProfile

A profile that certain accessories implement.

class HMNetworkConfigurationProfile

A profile that provides information about network protection for an accessory.

class HMCameraProfile

A camera profile that interacts with an accessory’s camera.

### Managing camera profiles

struct CameraView

A SwiftUI view into which a video stream or an image snapshot is rendered.

var cameraProfiles: [HMCameraProfile]?

An array of camera profiles implemented by the accessory.

class HMCameraProfile

A camera profile that interacts with an accessory’s camera.

class HMCameraView

The view into which a video stream or an image snapshot is rendered.

### Getting accessory state

var isReachable: Bool

A Boolean value indicating whether the accessory can be communicated with in the current network environment.

var isBlocked: Bool

A Boolean value indicating whether the accessory is blocked.

### Asking an accessory to identify itself

var supportsIdentify: Bool

A Boolean value that indicates whether the accessory supports the identify action.

func identify(completionHandler: ((any Error)?) -> Void)

Asks an accessory to identify itself.

### Controlling accessory features

var services: [HMService]

An array of services provided by the accessory.

class HMService

A controllable feature of an accessory, like a light attached to a garage door opener.

### Managing bridged accessories

var isBridged: Bool

A Boolean that indicates whether the accessory is accessed through a bridge.

var uniqueIdentifiersForBridgedAccessories: [UUID]?

An array of unique identifiers, each of which represents an accessory vended by the bridge.

var identifiersForBridgedAccessories: [UUID]?

An array of identifiers for accessories available through a bridge.

Deprecated

### Getting manufacturer information

var firmwareVersion: String?

The firmware version of the accessory.

var manufacturer: String?

The manufacturer of the accessory.

var model: String?

The model name of the accessory.

### Browsing for accessories

class HMAccessoryBrowser

A network browser you can use to discover new accessories in a home.

### Instance Properties

var matterNodeID: UInt64?

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

class HMService

A controllable feature of an accessory, like a light attached to a garage door opener.

class HMCharacteristic

A specific characteristic of a service, like the brightness of a dimmable light or its color temperature.

class HMMediaSourceDisplayOrderProfile

An interface from which to read and, if allowed by the accessory, update the ordering of input sources.

