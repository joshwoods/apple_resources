

- HomeKit
-  HMHomeDelegate 

Protocol

# HMHomeDelegate

An interface that communicates changes to a home’s configuration.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
protocol HMHomeDelegate : NSObjectProtocol
```

## Overview

Adopt this protocol to find out about changes made outside your app to a particular home, like when the home’s name changes, or when a room is added.

Changes that your app initiates—even those made asynchronously followed by a call to a completion handler—generate delegate callbacks in other apps, but not in your own. As a result, your app must update its internal data store or user interface from both the completion handler of an asynchronous call, and the delegate callback that corresponds to the same kind of change made by another app.

To be alerted about changes made to the overall list of homes, adopt the HMHomeManagerDelegate protocol. To find out about changes made to specific accessories, adopt the HMAccessoryDelegate protocol.

## Topics

### Observing Home Configuration

func homeDidUpdateName(HMHome)

Tells the delegate that a home’s name changed.

func home(HMHome, didAdd: HMAccessory)

Tells the delegate that a home added a new accessory.

func home(HMHome, didUpdate: HMRoom, for: HMAccessory)

Tells the delegate that a home assigned an accessory to a different room.

func home(HMHome, didRemove: HMAccessory)

Tells the delegate that a home removed an accessory.

func home(HMHome, didAdd: HMRoom)

Tells the delegate that a home added a new room.

func home(HMHome, didUpdateNameFor: HMRoom)

Tells the delegate that a home updated the name of one of its rooms.

func home(HMHome, didAdd: HMRoom, to: HMZone)

Tells the delegate that a home added a room to a zone.

func home(HMHome, didRemove: HMRoom, from: HMZone)

Tells the delegate that a home removed a room from a zone.

func home(HMHome, didRemove: HMRoom)

Tells the delegate that a home removed a room.

func home(HMHome, didAdd: HMZone)

Tells the delegate that a home added a new zone.

func home(HMHome, didUpdateNameFor: HMZone)

Tells the delegate that a home changed the name of a zone.

func home(HMHome, didRemove: HMZone)

Tells the delegate that a home removed a zone.

func home(HMHome, didAdd: HMUser)

Tells the delegate that a home added a user.

func home(HMHome, didRemove: HMUser)

Tells the delegate that a home removed a user.

func homeDidUpdateAccessControl(forCurrentUser: HMHome)

Tells the delegate that the access control for the current user has changed.

func home(HMHome, didUpdate: HMHomeHubState)

Tells the delegate that the state of the home hub has changed.

func homeDidUpdateSupportedFeatures(HMHome)

Tells the delegate that the home’s supported features changed.

enum HMHomeHubState

The possible states of the home hub.

### Observing Service Configuration

func home(HMHome, didAdd: HMServiceGroup)

Tells the delegate that a home added a service group.

func home(HMHome, didUpdateNameFor: HMServiceGroup)

Tells the delegate that a home updated the name of a service group.

func home(HMHome, didAdd: HMService, to: HMServiceGroup)

Tells the delegate that a home added a service to a service group.

func home(HMHome, didRemove: HMService, from: HMServiceGroup)

Tells the delegate that a home removed a service from a service group.

func home(HMHome, didRemove: HMServiceGroup)

Tells the delegate that a home removed a service group.

### Observing Action and Trigger Configuration

func home(HMHome, didAdd: HMActionSet)

Tells the delegate that a home added an action set.

func home(HMHome, didUpdateNameFor: HMActionSet)

Tells the delegate that a home updated the name of an action set.

func home(HMHome, didUpdateActionsFor: HMActionSet)

Tells the delegate that a home updated the actions for an action set.

func home(HMHome, didRemove: HMActionSet)

Tells the delegate that a home removed an action set.

func home(HMHome, didAdd: HMTrigger)

Tells the delegate that a home added a trigger.

func home(HMHome, didUpdateNameFor: HMTrigger)

Tells the delegate that a home updated the name of a trigger.

func home(HMHome, didUpdate: HMTrigger)

Tells the delegate that a home updated a trigger.

func home(HMHome, didRemove: HMTrigger)

Tells the delegate that a home removed a trigger.

### Observing Accessories

func home(HMHome, didEncounterError: any Error, for: HMAccessory)

Tells the delegate that a configured accessory encountered an error.

func home(HMHome, didUnblockAccessory: HMAccessory)

Tells the delegate that an accessory has been unblocked.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Keeping track of home configuration changes

var delegate: (any HMHomeDelegate)?

A delegate that receives updates on the state of the home.

