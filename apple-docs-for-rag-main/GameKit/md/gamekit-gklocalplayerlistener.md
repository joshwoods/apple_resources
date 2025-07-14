

- GameKit
-  GKLocalPlayerListener 

Protocol

# GKLocalPlayerListener

A protocol that handles events for Game Center players.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 3.0+

**tvOS, watchOS**

``` source
protocol GKLocalPlayerListener : GKChallengeListener, GKInviteEventListener, GKTurnBasedEventListener
```

**iOS, iPadOS, Mac Catalyst, macOS, visionOS**

``` source
protocol GKLocalPlayerListener : GKChallengeListener, GKInviteEventListener, GKSavedGameListener, GKTurnBasedEventListener
```

## Mentioned in 

Starting turn-based matches and passing turns between players

Finding multiple players for a game

Saving the player’s game data to an iCloud account

## Overview

Adopt the GKLocalPlayerListener protocol to listen for and handle a variety of Game Center events for player accounts instead of the individual GKChallengeListener, GKInviteEventListener, GKSavedGameListener, and GKTurnBasedEventListener protocols.

## Relationships

### Inherits From

- GKChallengeListener
- GKInviteEventListener
- GKSavedGameListener
- GKTurnBasedEventListener
- NSObjectProtocol

## See Also

### Players

Connecting players with their friends in your game

Give players the ability to connect and interact with friends in your game.

Saving the player’s game data to an iCloud account

Save game data during play or after a game in the player’s iCloud account that’s accessible from any device.

Protecting the player’s privacy using scoped identifiers

Use the scoped identifiers that GameKit provides you as player IDs when transmitting or saving player data.

class GKLocalPlayer

The local player who signs in to Game Center on the device running the game.

class GKPlayer

A remote player who the local player running your game can invite and communicate with through Game Center.

class GKBasePlayer

A class that provides common data and methods for the different player objects.

static let GKPlayerAuthenticationDidChangeNotificationName: NSNotification.Name

A notification that posts after GameKit authenticates the local player.

static let GKPlayerDidChangeNotificationName: NSNotification.Name

A notification that posts when a player object’s data changes.

