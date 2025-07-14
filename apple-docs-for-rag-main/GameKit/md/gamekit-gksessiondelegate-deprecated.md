

- GameKit
-  GKSessionDelegate Deprecated

Protocol

# GKSessionDelegate

An object implements the GKSessionDelegate protocol to control the behavior of a GKSession object. The delegate is called when other visible peers change their state relative to the session. It is also called to determine whether another peer is allowed to connect to the session.

macOS 10.8–10.10DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
protocol GKSessionDelegate : NSObjectProtocol
```

## Topics

### Observing Changes to Peers

func session(GKSession, peer: String, didChange: GKPeerConnectionState)

Received by the delegate when a peer changes state.

### Connection Requests from Other Peers

func session(GKSession, didReceiveConnectionRequestFromPeer: String)

Received by the delegate when a remote peer wants to create a connection to the session.

### Connection Errors

func session(GKSession, connectionWithPeerFailed: String, withError: any Error)

Received by the delegate when an attempt to connect to another peer failed.

func session(GKSession, didFailWithError: any Error)

Sent to the delegate when a serious error has occurred in the session.

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

protocol GKGameSessionEventListener

An event listener that handles game session events.

Deprecated

protocol GKLeaderboardViewControllerDelegate

The GKLeaderboardViewControllerDelegate protocol is implemented by delegates of the GKLeaderboardViewController class. The delegate is called when the player dismisses the leaderboard.

Deprecated

protocol GKPeerPickerControllerDelegate

The GKPeerPickerControllerDelegate protocol is implemented on an object to customize the behavior of a GKPeerPickerController object. The delegate is called by the peer picker to create a session object and to respond as the session is configured by the controller.

Deprecated

protocol GKTurnBasedEventHandlerDelegate

The GKTurnBasedEventHandlerDelegate protocol is implemented by an object to receive notifications events for turn-based matches. All methods are called on the main thread.

Deprecated

protocol GKVoiceChatClient

The GKVoiceChatClient protocol is implemented to control the behavior of the GKVoiceChatService object. The voice chat client has a number of responsibilities:

Deprecated

