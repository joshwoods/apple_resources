

- HomeKit
-  HMAccessoryDelegate 

Protocol

# HMAccessoryDelegate

A set of methods that defines the communication method for state updates from accessories to their delegates.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
protocol HMAccessoryDelegate : NSObjectProtocol, Sendable
```

## Overview

Adopt this protocol to find out about changes made outside your app to a specific accessory, like when the accessory’s name changes, or when a characteristic value changes.

Note

To receive accessory(_:service:didUpdateValueFor:) method calls for a particular characteristic, indicating when the characteristic value changes, you must first call the characteristic’s enableNotification(_:completionHandler:) method.

Changes that your app initiates—even those made asynchronously followed by a call to a completion handler—generate delegate callbacks in other apps, but not in your own. As a result, your app must update its internal data store or user interface from both the completion handler of an asynchronous call, and the delegate callback that corresponds to the same kind of change made by another app.

To find out about changes made to the accessory’s home, adopt the HMHomeDelegate protocol. To be alerted about changes made to the overall list of homes, adopt the HMHomeManagerDelegate protocol.

## Topics

### Observing accessories

func accessoryDidUpdateName(HMAccessory)

Informs the delegate when the name of the accessory is updated.

func accessoryDidUpdateReachability(HMAccessory)

Informs the delegate when the reachability of the accessory changes.

func accessoryDidUpdateServices(HMAccessory)

Informs the delegate when the services on the accessory have been updated.

func accessory(HMAccessory, didUpdateNameFor: HMService)

Informs the delegate when the name of a service is updated.

func accessory(HMAccessory, service: HMService, didUpdateValueFor: HMCharacteristic)

Informs the delegate of a change in value of a characteristic.

func accessory(HMAccessory, didUpdateAssociatedServiceTypeFor: HMService)

Informs the delegate when the associated service type of a service is modified.

func accessory(HMAccessory, didAdd: HMAccessoryProfile)

Informs the delegate when a profile is added to an accessory.

func accessory(HMAccessory, didRemove: HMAccessoryProfile)

Informs the delegate when a profile is removed from an accessory.

func accessory(HMAccessory, didUpdateFirmwareVersion: String)

Informs the delegate when firmwareVersion has been changed for an accessory.

## Relationships

### Inherits From

- NSObjectProtocol
- Sendable

## See Also

### Tracking changes to an accessory

var delegate: (any HMAccessoryDelegate)?

A delegate that receives updates on the state of the accessory.

