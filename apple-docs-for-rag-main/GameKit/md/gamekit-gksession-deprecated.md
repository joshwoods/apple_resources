

- GameKit
-  GKSession Deprecated

Class

# GKSession

A GKSession object provides the ability to discover and connect to nearby iOS devices using Bluetooth or Wi-fi.

macOS 10.8–10.10DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
class GKSession
```

## Overview

Sessions primarily work with *peers*. A peer is any iOS device made visible by creating and configuring a GKSession object. Each peer is identified by a unique identifier, called a peer id (peerID) string. Your application can use a peerID string to obtain a user-readable name for a remote peer and to attempt to connect to that peer. Similarly, your session’s peer ID is visible to other nearby peers. After a connection is established, your application uses the remote peer’s ID to address data packets that it wants to send.

Peers discover other peers by using a unique string to identify the service they implement, called a session ID (sessionID). Sessions can be configured to broadcast a session ID (as a *server*), to search for other peers advertising with that session ID (as a *client*), or to act as both a server and a client simultaneously (as a *peer*.

Your application controls the behavior of a session through a delegate that implements the GKSessionDelegate protocol. The delegate is called when remote peers are discovered, when those peers attempt to connect to the session, and when the state of a remote peer changes. Your application also provides a data handler to the session so that the session can forward data it receives from remote peers. The data handler can be a separate object or the same object as the delegate.

When Bluetooth is turned on, Wi-Fi download speeds drastically decrease while the device is searching for other Bluetooth enabled devices. After the Bluetooth discovery time has completed, Wi-Fi speeds return to normal.

GKSession methods are thread-safe and may be called from any thread. However, the session always calls its delegate on the main thread.

## Topics

### Creating a Session

init!(sessionID: String!, displayName: String!, sessionMode: GKSessionMode)

Initializes and returns a newly allocated session.

### Setting and Getting the Delegate

var delegate: (any GKSessionDelegate)!

The delegate of the session object.

### Searching for Other Peers

var isAvailable: Bool

A Boolean value that determines whether or not the session wants to connect to new peers.

### Obtaining Information About Other Peers

func peers(with: GKPeerConnectionState) -> [Any]!

Returns a list of peers in the specified connection state.

func displayName(forPeer: String!) -> String!

Returns a user-readable name for a peer.

### Connecting to a Remote Peer

func connect(toPeer: String!, withTimeout: TimeInterval)

Creates a connection to another iOS device.

func cancelConnect(toPeer: String!)

Cancels a pending request to connect to another iOS device.

### Receiving Connections from a Remote Peer

func acceptConnection(fromPeer: String!) throws

Called by the delegate to accept a connection request received from a remote peer.

func denyConnection(fromPeer: String!)

Called by the delegate to reject a connection request received from a remote peer.

### Working with Connected Peers

func setDataReceiveHandler(Any!, withContext: UnsafeMutableRawPointer!)

Sets the object that handles data received from other peers connected to the session.

func send(Data!, toPeers: [Any]!, with: GKSendDataMode) throws

Transmits a collection of bytes to a list of connected peers.

func sendData(toAllPeers: Data!, with: GKSendDataMode) throws

Transmits a collection of bytes to all connected peers.

var disconnectTimeout: TimeInterval

A time interval that expresses how long the session waits before it disconnects a nonresponsive peer.

func disconnectFromAllPeers()

Disconnects the session from all connected peers.

func disconnectPeer(fromAllPeers: String!)

Disconnects a connected peer from all peers connected to the session.

### Information about the Session

var displayName: String!

The name of the user.

var peerID: String!

A string that identifies your session to other peers.

var sessionID: String!

A string used to filter the list of peers who are allowed to see your session.

var sessionMode: GKSessionMode

The mode the session uses to find other peers.

### Constants

enum GKSendDataMode

The mechanism used to transmit data to other peers.

enum GKSessionMode

Modes that determine how a session interacts with other peers.

enum GKPeerConnectionState

The state of a peer known to the session.

The Session Error Domain

The GKSession error domain.

enum Code

Error codes for the session error domain.

struct GKSessionError

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

### Deprecated classes

class GKAchievementViewController

An `GKAchievementViewController` object provides a standard user interface to display achievement progress for the local player. If the GKGameCenterViewController class is available, you should use it instead.

Deprecated

class GKChallengeEventHandler

The `GKChallengeEventHandler` class is used to respond to events related to challenges sent or received by the local player.

Deprecated

class GKChallengesViewControllerDeprecated

class GKCloudPlayer

The object representing the currently signed-in iCloud user.

Deprecated

class GKGameSession

A game session you can use to save game data, invite other players, and create turn-based and real-time game apps.

Deprecated

class GKGameSessionSharingViewController

A user interface you can use to invite other users into a tvOS game session.

Deprecated

class GKFriendRequestComposeViewController

Your game uses the `GKFriendRequestComposeViewController` class to present a screen that allows the local player to send friend requests to other players.

Deprecated

class GKLeaderboardViewController

The `GKLeaderboardViewController` class provides a standard user interface that displays leaderboard scores to the player. If the GKGameCenterViewController class is available, you should use it instead.

Deprecated

class GKPeerPickerController

Provides a standard user interface to allow one iOS device to discover and connect to another.

Deprecated

class GKScore

An object containing information for a score that was earned by the player.

Deprecated

class GKTurnBasedEventHandler

The GKTurnBasedEventHandler class is used to respond to important messages related to turn-based matches. To use it, call the shared() class method to get the singleton instance and assign an object that implements the GKTurnBasedEventHandlerDelegate protocol to its delegate property. All methods are called on the main thread.

Deprecated

class GKVoiceChat

A voice channel that allows players to speak with each other in a multiplayer game.

Deprecated

class GKVoiceChatService

The GKVoiceChatService class allows your application to connect two iOS devices into a voice chat.

Deprecated

