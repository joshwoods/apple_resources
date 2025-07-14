

- HomeKit
-  HMAddAccessoryRequest 

Class

# HMAddAccessoryRequest

A request to add an accessory to a particular home.

iOS 8.0+iPadOS 8.0+visionOS 1.0+

``` source
class HMAddAccessoryRequest
```

## Overview

An HMAddAccessoryRequest instance describes an accessory that your app should add to a home. HomeKit calls your home manager delegate’s homeManager(_:didReceiveAddAccessoryRequest:) method with a request.

Use the request’s accessoryName and accessoryCategory properties to obtain a token by negotiating with the accessory outside of HomeKit. If the requiresSetupPayloadURL property is `true`, also prepare a setup payload URL. Then create a setup payload with either the makePayload(url:ownershipToken:) or makePayload(ownershipToken:) method. Complete the request by calling the addAndSetupAccessories(with:completionHandler:) method on the request’s home property.

## Topics

### Characterizing the Request

var home: HMHome

The home to which to add the accessory.

var accessoryCategory: HMAccessoryCategory

The category of the accessory to add.

var accessoryName: String

The name of the accessory to add.

var requiresOwnershipToken: Bool

An indication of whether the add operation requires an ownership token.

Deprecated

var requiresSetupPayloadURL: Bool

An indication of whether the add operation requires a setup payload URL.

### Creating a Payload

func makePayload(ownershipToken: HMAccessoryOwnershipToken) -> HMAccessorySetupPayload?

Builds an accessory setup payload with the given ownership token.

func makePayload(url: URL, ownershipToken: HMAccessoryOwnershipToken) -> HMAccessorySetupPayload?

Builds an accessory setup payload with the given setup payload URL and ownership token.

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

## See Also

### Adding accessories

func homeManager(HMHomeManager, didReceiveAddAccessoryRequest: HMAddAccessoryRequest)

Tells the delegate to add an accessory to a home by using a setup payload.

