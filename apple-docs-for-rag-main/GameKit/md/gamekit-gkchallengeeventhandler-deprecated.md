

- GameKit
-  GKChallengeEventHandler Deprecated

Class

# GKChallengeEventHandler

The `GKChallengeEventHandler` class is used to respond to events related to challenges sent or received by the local player.

macOS 10.8–10.10DeprecatedvisionOS 1.0–1.0Deprecated

``` source
class GKChallengeEventHandler
```

Deprecated

Use the GKChallengeListener protocol and register a listener with GKLocalPlayer instead.

## Overview

Important

Your game must authenticate a local player before you can use any Game Center classes. If there is no authenticated player, your game receives a GKError.Code.notAuthenticated error. For more information, see Authenticating a player.

To use it, call the challengeEventHandler class method to get the Singleton instance and assign an object that implements the GKChallengeEventHandlerDelegate protocol to its delegate property. You should assign a challenge event handler immediately after the local player has been authenticated, because your game may have been launched in response to a challenge notification being received by the player.

## Topics

### Getting and Setting the Delegate

var delegate: (any GKChallengeEventHandlerDelegate)!

The delegate for the event handler.

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

