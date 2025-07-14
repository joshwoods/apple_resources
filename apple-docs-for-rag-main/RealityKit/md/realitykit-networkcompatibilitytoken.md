

- RealityKit
-  NetworkCompatibilityToken 

Class

# NetworkCompatibilityToken

An opaque token used to check the networking compatibility between two peers in a multipeer connection.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOS 10.15.4+visionOS

``` source
final class NetworkCompatibilityToken
```

## Overview

RealityKit apps running on incompatible versions of RealityKit can’t connect and sync over the network. Use NetworkCompatibilityToken to check if two peers can synchronize RealityKit scenes over the network. With this class, host applications can prevent incompatible clients from joining.

Client apps send a copy of their token to the host when attempting to connect to a host app. The host deserializes that token and calls compatibilityWith(_:) on NetworkCompatibilityToken.local. If compatibilityWith(_:) returns NetworkCompatibilityToken.Compatibility.compatible, the client and host can sync and it’s safe to proceed with the connection. If compatibilityWith(_:) returns any other value, the client that’s attempting to connect is incompatible and should be ignored.

A client running a MCNearbyServiceAdvertiser, for example, writes its own token into its discoveryInfo dictionary. When the host (running a MCNearbyServiceBrowser) discovers that client, it deserializes the client’s token from the `discoverInfo` dictionary and uses it to check compatibility before inviting the client to the MCSession.

Note

Even if two peers are compatible, scene synchronization can fail for other reasons, such as packet corruption or a poor network connection.

## Topics

### Retrieving tokens

static let local: NetworkCompatibilityToken

A token containing the local peer’s networking compatibility info.

### Checking compatibility

func compatibilityWith(NetworkCompatibilityToken) -> NetworkCompatibilityToken.Compatibility

Compares network compatibility tokens between the local device and another device.

### Serializing tokens

init(from: any Decoder) throws

Creates a new instance from a decoder.

func encode(to: any Encoder) throws

Writes the token’s data into an encoder.

### Enumerations

enum Compatibility

Indicates whether two devices running RealityKit are compatible and able to connect and sync scenes.

## Relationships

### Conforms To

- Decodable
- Encodable

## See Also

### Multipeer synchronization

Loading remote assets in multiplayer apps

Ensure assets load on all connected peers before using them.

class MultipeerConnectivityService

A service that provides scene synchronization among all peers in a multipeer connectivity session.

enum Compatibility

Indicates whether two devices running RealityKit are compatible and able to connect and sync scenes.

protocol TransientComponent

An interface for components that aren’t saved to file or cloned.

