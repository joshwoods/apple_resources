

- CarKey
-  CarKeyRemoteControl 

Class

# CarKeyRemoteControl

The object you use to start a new vehicle-related session.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.3+watchOS 9.0+

``` source
class CarKeyRemoteControl
```

## Overview

Use a CarKeyRemoteControl object to create the session your app uses to communicate with the vehicles your company manufactures. You don’t create an instance of this object. Instead, call the start(delegate:subscriptionRange:with:) class method to request a new session object. The system retrieves the relevant vehicle information from person’s Apple Wallet and adds vehicles that match your company’s make to the session.

Start a new session only when your app is running in the foreground. If your app enters the background, end the current session and start a new one when your app returns to the foreground.

## Topics

### Creating the Session Object

class func start(delegate: any CarKeyRemoteControlSessionDelegate, subscriptionRange: ClosedRange&lt;Int>?, with: DispatchQueue?) async throws -> CarKeyRemoteControlSession

Creates and returns a new session object to access the provisioned vehicles.

## See Also

### Setup

class CarKeyRemoteControlSession

The object that manages communication with the vehicles you manufacture.

protocol CarKeyRemoteControlSessionDelegate

An interface you use to receive session- and vehicle-related information from the system.

struct VehicleReport

A type that contains information about a vehicle configured for remote keyless entry in the user’s Apple Wallet.

