

- GameKit
-  GKGameSessionSharingViewController Deprecated

Class

# GKGameSessionSharingViewController

A user interface you can use to invite other users into a tvOS game session.

tvOS 10.0–12.0Deprecated

``` source
@MainActor
class GKGameSessionSharingViewController
```

Deprecated

For real-time matches, use GKMatchmakerViewController. For turn-based matches, use GKTurnBasedMatchmakerViewController.

## Overview

The sharing view controller on tvOS presents a user’s Game Center friend list, along with other people with whom the user has recently played the game. Users can select a person from the list and send them an invite using the Send button.

Note

Currently, the a user’s Game Center friend’s list is frozen and users will no longer be able to add friends to the list.

## Topics

### Presenting the Share UI

init(session: GKGameSession)

Creates a new sharing view controller for a specified session.

### Accessing Share View Controller Properties

var delegate: (any GKGameSessionSharingViewControllerDelegate)?

The delegate for the sharing view controller.

protocol GKGameSessionSharingViewControllerDelegate

A protocol you implement to respond to changes to a sharing user interface.

var session: GKGameSession

The game session associated with the view controller.

## Relationships

### Inherits From

- UIViewController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSExtensionRequestHandling
- NSObjectProtocol
- Sendable
- UIAppearanceContainer
- UIContentContainer
- UIFocusEnvironment
- UIResponderStandardEditActions
- UIStateRestoring
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

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

