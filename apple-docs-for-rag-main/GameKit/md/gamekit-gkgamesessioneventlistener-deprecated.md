

- GameKit
-  GKGameSessionEventListener Deprecated

Protocol

# GKGameSessionEventListener

An event listener that handles game session events.

iOS 10.0–12.0DeprecatediPadOS 10.0–12.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.12–10.14DeprecatedtvOS 10.0–12.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
protocol GKGameSessionEventListener : NSObjectProtocol
```

## Topics

### Changing Player Status

func session(GKGameSession, didAdd: GKCloudPlayer)

Tells the listener a new player has been added to a game session.

func session(GKGameSession, didRemove: GKCloudPlayer)

Tells the listener a player left a game session.

func session(GKGameSession, player: GKCloudPlayer, didChange: GKConnectionState)

Tells the listener a player’s connection state has changed.

enum GKConnectionState

Possible connection states for a player

### Transferring Data

func session(GKGameSession, didReceive: Data, from: GKCloudPlayer)

Tells the listener the player received data from another player.

func session(GKGameSession, didReceiveMessage: String, with: Data, from: GKCloudPlayer)

Tells the listener a player has received a message from another player.

func session(GKGameSession, player: GKCloudPlayer, didSave: Data)

Tells the listener data was saved by a player.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Deprecated protocols

protocol GKAchievementViewControllerDelegate

An object implementing the GKAchievementViewControllerDelegate protocol is called when the user dismisses the achievements view controller. Typically, this protocol is implemented by the object in your game that originally displayed the achievements user interface.

Deprecated

protocol GKChallengeEventHandlerDelegate

You implement the GKChallengeEventHandlerDelegate delegate to control how challenges are displayed in your game.

Deprecated

protocol GKChallengesViewControllerDelegateDeprecated

protocol GKFriendRequestComposeViewControllerDelegate

The GKFriendRequestComposeViewControllerDelegate protocol is implemented by delegates of the GKFriendRequestComposeViewController class. The delegate is called when the player dismisses the friend request.

Deprecated

protocol GKLeaderboardViewControllerDelegate

The GKLeaderboardViewControllerDelegate protocol is implemented by delegates of the GKLeaderboardViewController class. The delegate is called when the player dismisses the leaderboard.

Deprecated

protocol GKPeerPickerControllerDelegate

The GKPeerPickerControllerDelegate protocol is implemented on an object to customize the behavior of a GKPeerPickerController object. The delegate is called by the peer picker to create a session object and to respond as the session is configured by the controller.

Deprecated

protocol GKSessionDelegate

An object implements the GKSessionDelegate protocol to control the behavior of a GKSession object. The delegate is called when other visible peers change their state relative to the session. It is also called to determine whether another peer is allowed to connect to the session.

Deprecated

protocol GKTurnBasedEventHandlerDelegate

The GKTurnBasedEventHandlerDelegate protocol is implemented by an object to receive notifications events for turn-based matches. All methods are called on the main thread.

Deprecated

protocol GKVoiceChatClient

The GKVoiceChatClient protocol is implemented to control the behavior of the GKVoiceChatService object. The voice chat client has a number of responsibilities:

Deprecated

