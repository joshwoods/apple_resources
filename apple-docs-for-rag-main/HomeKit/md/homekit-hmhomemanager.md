

- HomeKit
-  HMHomeManager 

Class

# HMHomeManager

The manager for a collection of one or more of a user’s homes.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
class HMHomeManager
```

## Mentioned in 

Enabling HomeKit in your app

## Overview

HomeKit stores the user’s home automation information in a database that’s shared among Apple’s built-in iOS Home app, your HomeKit-enabled app, and apps from other developers. All these apps access the database as peers using the HomeKit framework.

Each app creates a single HMHomeManager instance to coordinate its HomeKit-related activities. The manager’s homes array gives your app access to a collection of HMHome instances that represent the user’s homes. These in turn contain references to the home automation accessories that your app can inspect and control.

Adopt the HMHomeManagerDelegate protocol in your app to stay informed of any changes to the set of homes made outside your app.

## Topics

### Inspecting authorization status

var authorizationStatus: HMHomeManagerAuthorizationStatus

The current state of the app’s access to home data.

struct HMHomeManagerAuthorizationStatus

The possible home-access states.

### Working with the home layout

var homes: [HMHome]

An array of all homes managed by this home manager.

class HMHome

The primary unit of living space, typically composed of rooms organized into zones.

### Keeping track of connected homes

var delegate: (any HMHomeManagerDelegate)?

A delegate that receives updates on the collection of homes.

protocol HMHomeManagerDelegate

An interface the home manager uses to communicate changes to the state of the home network.

### Adding and removing homes

func addHome(withName: String, completionHandler: (HMHome?, (any Error)?) -> Void)

Adds a new home to this home manager.

func removeHome(HMHome, completionHandler: ((any Error)?) -> Void)

Removes a home from this home manager.

### Managing the primary home

var primaryHome: HMHome?

The primary home managed by this home manager.

Deprecated

func updatePrimaryHome(HMHome, completionHandler: ((any Error)?) -> Void)

Updates the primary home of this home manager.

Deprecated

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

### Home Manager

Configuring a home automation device

Give users a familiar experience when they manage HomeKit accessories.

Testing your app with the HomeKit Accessory Simulator

Install the HomeKit Accessory Simulator to help you debug your HomeKit-enabled app.

