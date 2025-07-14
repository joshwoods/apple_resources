

- CarKey
-  CarKeyRemoteControlSession 

Class

# CarKeyRemoteControlSession

The object that manages communication with the vehicles you manufacture.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.3+watchOS 9.0+

``` source
class CarKeyRemoteControlSession
```

## Overview

A `CarKeyRemoteControlSession` object coordinates interactions between your app and your company’s make of vehicles. This object works with the system to transmit data securely to and from a vehicle, and to report results back to your app. Use this object to send commands or data directly to a vehicle, and to get information about the available vehicles and their current configuration.

Don’t create this object directly. Instead, call the start(delegate:subscriptionRange:with:) method to create a new session object. When you finish interacting with the vehicle, call the session’s end() method to close out the session and prevent further access. You can have only one active session at a time. If you try to start a second session, start(delegate:subscriptionRange:with:) doesn’t return until the currently active session becomes invalid.

When you configure a new session, provide a delegate object to receive data from vehicle-initiated transfers. The system also uses your delegate notify you when the configuration of a vehicle changes. For example, it lets you know when connectivity to the vehicle changes. The delegate must adopt the CarKeyRemoteControlSessionDelegate protocol.

Note

If your app has an active session, the system automatically ends that session when your app enters the background. Upon reentering the foreground, you must create a new session to communicate with your vehicle again.

## Topics

### Performing Vehicle-Related Actions

func perform(RemoteKeylessEntryAction) throws -> RemoteKeylessEntryAction.ExecutionRequest

Sends a request to the vehicle to perform a one-time action.

func perform(RemoteKeylessEntryEnduringAction) throws -> RemoteKeylessEntryEnduringAction.EnduringExecutionRequest

Sends a request to the vehicle to start an action that has a separate stopping point.

Deprecated

### Sending Data to the Vehicle

func sendPassthroughData(Data, toVehicle: String) throws

Sends the specified custom data to the vehicle.

### Closing the Session

func end() throws

Ends the session and stops the delivery of notifications for all vehicles in the session.

### Getting Vehicle Information

var vehicleReports: [VehicleReport]

The configuration details of the provisioned vehicles that match your company’s make.

func isPassiveEntryAvailable(forVehicle: String) throws -> Bool

Returns a Boolean value that indicates whether passive entry is currently available for the specified vehicle.

### Structures

struct Attestation

Object representing an attestation and related data

### Instance Methods

func perform(RemoteKeylessEntryConfigurableEnduringAction, continuationStrategy: CarKeyRemoteControlSession.ContinuationStrategy) throws -> RemoteKeylessEntryConfigurableEnduringAction.EnduringExecutionRequest

Sends a request to the vehicle to start an action that has a separate stopping point, and optionally allows your app to have control over incoming continuation requests and to exchange data during the execution of the action.

func sign(data: Data, forVehicle: String) throws -> CarKeyRemoteControlSession.Attestation

Sign data with the endpoint.SK identified by vehicleIdentifier as described in the section “OEM App Data Attestation” of the Car Connectivity Consortium Digital Key Release 3.0 specification.

### Enumerations

enum ContinuationStrategy

Strategy to use on reception of a continuation request.

## See Also

### Setup

class CarKeyRemoteControl

The object you use to start a new vehicle-related session.

protocol CarKeyRemoteControlSessionDelegate

An interface you use to receive session- and vehicle-related information from the system.

struct VehicleReport

A type that contains information about a vehicle configured for remote keyless entry in the user’s Apple Wallet.

