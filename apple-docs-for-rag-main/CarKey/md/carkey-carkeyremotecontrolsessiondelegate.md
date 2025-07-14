

- CarKey
-  CarKeyRemoteControlSessionDelegate 

Protocol

# CarKeyRemoteControlSessionDelegate

An interface you use to receive session- and vehicle-related information from the system.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.3+watchOS 9.0+

``` source
protocol CarKeyRemoteControlSessionDelegate
```

## Overview

The system uses the CarKeyRemoteControlSessionDelegate protocol to notify your app asynchronously when something happens. Adopt this protocol in one of your objects and detect when the system invalidates the session. If your vehicle is capable of sending data to your app, you also use this protocol to receive any data the vehicle sends.

## Topics

### Receiving Data from the Vehicle

func remoteControlSession(CarKeyRemoteControlSession, vehicleDidUpdateReport: VehicleReport)

Notifies your delegate object that the status of the specified vehicle changed.

**Required**

func remoteControlSession(CarKeyRemoteControlSession, didReceivePassthroughData: Data, fromVehicle: String)

Notifies the delegate object that the vehicle sent passthrough data for you to handle.

**Required**

### Handling Session Invalidation

func remoteControlSession(CarKeyRemoteControlSession, didInvalidateWithError: CarKeyErrorCode)

Notifies your delegate object that the session become invalid for the specified reason.

**Required**

### Instance Methods

func remoteControlSession(CarKeyRemoteControlSession, didCreateKey: String, forVehicle: String)

Called to notify your app when a new key has been created.

**Required** Default implementation provided.

## See Also

### Setup

class CarKeyRemoteControl

The object you use to start a new vehicle-related session.

class CarKeyRemoteControlSession

The object that manages communication with the vehicles you manufacture.

struct VehicleReport

A type that contains information about a vehicle configured for remote keyless entry in the user’s Apple Wallet.

