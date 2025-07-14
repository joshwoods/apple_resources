

- GameKit
-  GKGameSession Deprecated

Class

# GKGameSession

A game session you can use to save game data, invite other players, and create turn-based and real-time game apps.

iOS 10.0–12.0DeprecatediPadOS 10.0–12.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.12–10.14DeprecatedtvOS 10.0–12.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
class GKGameSession
```

Deprecated

For real-time matches, use GKMatchmakerViewController. For turn-based matches, use GKTurnBasedMatchmakerViewController.

## Overview

Use a `GKGameSession` object to play turn-based and real-time games in iCloud. Every instance of a game session resides inside of an iCloud container. You can create multiple sessions for a single app, allowing players to play several games at once. All of the information for a game session is saved in the owner’s iCloud.

Each session can contain a maximum of 100 players. Inside of a session, up to 16 of those players can be connected to each other in real-time. The 16 connected players can be selected from any of the 100 players in the session. You can change a connected player with another player in the session at any time.

After a game session is created, you can save game data in iCloud. Each game session can save a maximum of 512KB data. This prevents games from using a large about of space in a user’s iCloud account. This data can be loaded, edited, and saved by anyone in the game session, providing your app provides this behavior. You must ensure that you delete a game session from a user’s iCloud after a game is over, otherwise the session will stay in the user’s iCloud forever. Game sessions are not automatically removed after a set amount of time. They can only be actively removed.

## Topics

### Creating and Loading Game Sessions

class func createSession(inContainer: String?, withTitle: String, maxConnectedPlayers: Int, completionHandler: (GKGameSession?, (any Error)?) -> Void)

Creates a new game session inside of an iCloud container.

class func load(withIdentifier: String, completionHandler: (GKGameSession?, (any Error)?) -> Void)

Loads a specific game session.

class func loadSessions(inContainer: String?, completionHandler: ([GKGameSession]?, (any Error)?) -> Void)

Retrieves all of the game sessions associated with a container.

class func remove(withIdentifier: String, completionHandler: ((any Error)?) -> Void)

Removes the specified game session.

### Accessing Information About a Game Session

var identifier: String

A unique identifier for a game session.

var lastModifiedDate: Date

The date that the game session was last modified.

var lastModifiedPlayer: GKCloudPlayer

The last player to modify the game session.

var maxNumberOfConnectedPlayers: Int

The maximum number of players allowed to connect to the game session at the same time.

var owner: GKCloudPlayer

A player object that represents the owner of the game session.

var players: [GKCloudPlayer]

An array of player objects associated with the game session.

var title: String

The title of the game session.

### Inviting Players to a Game Session

func getShareURL(completionHandler: (URL?, (any Error)?) -> Void)

Retrieves the URL used to share a game session.

### Saving and Loading Data

func loadData(completionHandler: (Data?, (any Error)?) -> Void)

Retrieves the game data from the current game session.

func save(Data, completionHandler: (Data?, (any Error)?) -> Void)

Saves the current game session data.

### Listening for Events

class func add(listener: any GKGameSessionEventListener)

Adds a new event listener object.

class func remove(listener: any GKGameSessionEventListener)

Stops listening to the event listener object.

### Connecting Players for Real-Time Communication

func setConnectionState(GKConnectionState, completionHandler: ((any Error)?) -> Void)

Sets the connection state for the player.

func players(with: GKConnectionState) -> [GKCloudPlayer]

Retrieves a list of players with the specified connection state.

func send(Data, with: GKTransportType, completionHandler: ((any Error)?) -> Void)

Sends the indicated data to all connected players.

enum GKTransportType

The mechanism used to send messages to other players in a game session.

### Communicating Between Players

var badgedPlayers: [GKCloudPlayer]

An array containing all of the currently badged players.

func clearBadge(for: [GKCloudPlayer], completionHandler: ((any Error)?) -> Void)

Clears the badge from the designated players.

func sendMessage(withLocalizedFormatKey: String, arguments: [String], data: Data?, to: [GKCloudPlayer], badgePlayers: Bool, completionHandler: ((any Error)?) -> Void)

Sends a message to players in a game session.

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

class GKSession

A GKSession object provides the ability to discover and connect to nearby iOS devices using Bluetooth or Wi-fi.

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

