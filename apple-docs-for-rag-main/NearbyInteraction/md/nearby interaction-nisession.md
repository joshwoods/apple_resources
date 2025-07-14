

- Nearby Interaction
-  NISession 

Class

# NISession

An object that identifies a unique connection between two peer devices.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+watchOS 7.3+

``` source
class NISession
```

## Mentioned in 

Initiating and maintaining a session

Discovering peers with Multipeer Connectivity

Extending advanced direction finding and ranging

## Overview

This class represents the central mechanism to interact with nearby objects, for example, a peer Apple device or third-party accessory. After creating an NISession for a nearby object, the app interacts with the object by receiving NISessionDelegate callbacks.

One session represents an interaction between the user and a single nearby object. To interact with multiple nearby objects, create a separate session for each.

For more information, see Initiating and maintaining a session.

## Topics

### Ensuring feature support

class var deviceCapabilities: any NIDeviceCapability

An object that communicates the device’s supported framework features.

protocol NIDeviceCapability

An interface that adds Boolean values that indicate an interaction session feature support.

### Connecting to A Peer Device

var discoveryToken: NIDiscoveryToken?

A temporary, random identifier for a device.

class NIDiscoveryToken

An object that uniquely identifies a peer that participates in an interaction session.

func run(NIConfiguration)

Starts a session with a nearby peer.

var configuration: NIConfiguration?

The configuration run by the session.

var delegateQueue: dispatch_queue_t?

The dispatch queue on which the session invokes delegate callbacks.

### Managing life cycle

var delegate: (any NISessionDelegate)?

An object that the framework notifies of session events.

func pause()

Stops sending distance and direction updates to the peer.

func invalidate()

Stops a running session.

### Utilizing Camera Assistance

func setARSession(ARSession)

Provides the framework with an existing AR session to use for Camera Assistance.

func worldTransform(for: NINearbyObject) -> simd_float4x4?

Returns a world transform to integrate a nearby object in an AR experience.

### Deprecated

class var isSupported: Bool

A Boolean value that indicates whether the device supports basic interaction-session functionality.

Deprecated

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

### Setup

Initiating and maintaining a session

Measure the relative position of a nearby device and coach the user to sustain interaction.

