

- GameKit
-  GKChallengesViewController Deprecated

Class

# GKChallengesViewController

macOS 10.8–10.10Deprecated

``` source
@MainActor
class GKChallengesViewController
```

Deprecated

No longer supported

## Topics

### Getting the Delegate

var challengeDelegate: (any GKChallengesViewControllerDelegate)!

## Relationships

### Inherits From

- NSViewController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- GKViewController
- Hashable
- NSCoding
- NSEditor
- NSExtensionRequestHandling
- NSObjectProtocol
- NSSeguePerforming
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
- Sendable

## See Also

### Deprecated classes

class GKAchievementViewController

An `GKAchievementViewController` object provides a standard user interface to display achievement progress for the local player. If the GKGameCenterViewController class is available, you should use it instead.

Deprecated

class GKChallengeEventHandler

The `GKChallengeEventHandler` class is used to respond to events related to challenges sent or received by the local player.

Deprecated

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

