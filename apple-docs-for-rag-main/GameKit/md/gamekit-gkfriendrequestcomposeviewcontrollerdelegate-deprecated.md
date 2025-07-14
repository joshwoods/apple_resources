

- GameKit
-  GKFriendRequestComposeViewControllerDelegate Deprecated

Protocol

# GKFriendRequestComposeViewControllerDelegate

The GKFriendRequestComposeViewControllerDelegate protocol is implemented by delegates of the GKFriendRequestComposeViewController class. The delegate is called when the player dismisses the friend request.

iOS 4.2–10.0DeprecatediPadOS 4.2–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.8–10.12DeprecatedvisionOS 1.0–1.0Deprecated

``` source
protocol GKFriendRequestComposeViewControllerDelegate
```

Deprecated

No longer supported.

## Topics

### Responding to User Events

func friendRequestComposeViewControllerDidFinish(GKFriendRequestComposeViewController)

Called when the player dismisses the request.

**Required**

## See Also

### Deprecated protocols

protocol GKAchievementViewControllerDelegate

An object implementing the GKAchievementViewControllerDelegate protocol is called when the user dismisses the achievements view controller. Typically, this protocol is implemented by the object in your game that originally displayed the achievements user interface.

Deprecated

protocol GKChallengeEventHandlerDelegate

You implement the GKChallengeEventHandlerDelegate delegate to control how challenges are displayed in your game.

Deprecated

protocol GKChallengesViewControllerDelegateDeprecated

protocol GKGameSessionEventListener

An event listener that handles game session events.

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

