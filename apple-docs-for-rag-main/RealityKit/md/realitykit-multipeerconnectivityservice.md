

- RealityKit
-  MultipeerConnectivityService 

Class

# MultipeerConnectivityService

A service that provides scene synchronization among all peers in a multipeer connectivity session.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+

``` source
class MultipeerConnectivityService
```

## Overview

RealityKit uses this class to automatically sync scenes with other connected devices running the same app. It leverages the Multipeer Connectivity framework to automatically keep the scenes of all connected devices synchronized. To sync a RealityKit scene, create a MultipeerConnectivityService object initialized with an MCSession and assign it to your scene’s synchronizationService property.

```
let peerID = MCPeerID(displayName: UIDevice.current.name)
let session = MCSession(peer: peerID, securityIdentity: nil, encryptionPreference: .required)
arView.scene.synchronizationService = try?
MultipeerConnectivityService(session: self.session)
```

For more information on browsing for, and connecting to, other devices, see Multipeer Connectivity.

## Topics

### Creating a connectivity service

init(session: MCSession) throws

Creates a new connectivity service.

### Getting the session

let session: MCSession

The multipeer connectivity session used by the service.

### Managing ownership

func owner(of: Entity) -> (any SynchronizationPeerID)?

Gets the device that owns a given entity.

func giveOwnership(of: Entity, toPeer: any SynchronizationPeerID) -> Bool

Transfers ownership of the given entity to the named network device.

### Finding an entity

func entity(for: MultipeerConnectivityService.Identifier) -> Entity?

Gets the entity with the given identifier.

### Pausing and resuming

func stopSync()

Stops multipeer synchronization.

func startSync()

Begins multipeer synchronization.

### Configuring the session

func setHandshake(count: UInt32, timeoutMs: UInt32)

Configures handshake and timeout settings.

## Relationships

### Conforms To

- SynchronizationService

## See Also

### Multipeer synchronization

Loading remote assets in multiplayer apps

Ensure assets load on all connected peers before using them.

class NetworkCompatibilityToken

An opaque token used to check the networking compatibility between two peers in a multipeer connection.

enum Compatibility

Indicates whether two devices running RealityKit are compatible and able to connect and sync scenes.

protocol TransientComponent

An interface for components that aren’t saved to file or cloned.

