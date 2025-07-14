

- GameKit
-  GKBasePlayer 

Class

# GKBasePlayer

A class that provides common data and methods for the different player objects.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class GKBasePlayer
```

## Overview

GKBasePlayer is the abstract superclass for the classes that represent the local player running your app and remote players who may join their games. Use the GKLocalPlayer subclass to authenticate the local player who runs your app on their device. Then you can access the local player’s nickname, avatar, leaderboards, and achievements. You can also invite other players (GKPlayer objects), and send information between players.

## Topics

### Identifying a Player

var displayName: String?

The Game Center profile name for a player.

var playerID: String?

A unique identifier for a player.

Deprecated

## Relationships

### Inherits From

- NSObject

### Inherited By

- GKCloudPlayer
- GKPlayer

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
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

protocol GKLocalPlayerListener

A protocol that handles events for Game Center players.

static let GKPlayerAuthenticationDidChangeNotificationName: NSNotification.Name

A notification that posts after GameKit authenticates the local player.

static let GKPlayerDidChangeNotificationName: NSNotification.Name

A notification that posts when a player object’s data changes.

