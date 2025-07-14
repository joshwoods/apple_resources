

- GameKit
-  GKMatchDelegate 

Protocol

# GKMatchDelegate

An object that receives connection status and data transmitted in a multiplayer game.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
protocol GKMatchDelegate : NSObjectProtocol
```

## Topics

### Receiving Data from Other Players

func match(GKMatch, didReceive: Data, forRecipient: GKPlayer, fromRemotePlayer: GKPlayer)

Processes the data sent from one player to another.

func match(GKMatch, didReceive: Data, fromRemotePlayer: GKPlayer)

Processes the data sent from another player to the local player.

### Receiving State Notifications About Other Players

func match(GKMatch, player: GKPlayer, didChange: GKPlayerConnectionState)

Handles when players connect or disconnect from a match.

enum GKPlayerConnectionState

The possible states of a connection to a match.

### Handling Errors

func match(GKMatch, didFailWithError: (any Error)?)

Handles the local player’s connection errors to a match.

### Reinviting a Player

func match(GKMatch, shouldReinviteDisconnectedPlayer: GKPlayer) -> Bool

Determines whether the local player should reinvite another player who disconnected from a two-player match.

### Deprecated Methods and Properties

func match(GKMatch, player: String, didChange: GKPlayerConnectionState)

Handles when a player connects or disconnects from a match.

Deprecated

func match(GKMatch, didReceive: Data, fromPlayer: String)

Handles when a player receives data in a match.

Deprecated

func match(GKMatch, shouldReinvitePlayer: String) -> Bool

Handles when a player disconnects from a two-player match.

Deprecated

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Setting the delegate

var delegate: (any GKMatchDelegate)?

The delegate that handles communication between players in a match.

