

- Nearby Interaction
-  NIDiscoveryToken 

Class

# NIDiscoveryToken

An object that uniquely identifies a peer that participates in an interaction session.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+watchOS 7.3+

``` source
class NIDiscoveryToken
```

## Mentioned in 

Extending advanced direction finding and ranging

## Overview

Use `NIDiscoveryToken` to determine the peer device’s nearby interaction capabilities by examining the deviceCapabilities that describes the available capabilities on a person’s device.

## Topics

### Understanding device capabilities

var deviceCapabilities: any NIDeviceCapability

A protocol object that describes the nearby interaction capabilities of a person’s device.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Connecting to A Peer Device

var discoveryToken: NIDiscoveryToken?

A temporary, random identifier for a device.

func run(NIConfiguration)

Starts a session with a nearby peer.

var configuration: NIConfiguration?

The configuration run by the session.

var delegateQueue: dispatch_queue_t?

The dispatch queue on which the session invokes delegate callbacks.

