

- GameKit
-  GKPeerPickerControllerDelegate Deprecated

Protocol

# GKPeerPickerControllerDelegate

The GKPeerPickerControllerDelegate protocol is implemented on an object to customize the behavior of a GKPeerPickerController object. The delegate is called by the peer picker to create a session object and to respond as the session is configured by the controller.

visionOS 1.0–1.0Deprecated

``` source
protocol GKPeerPickerControllerDelegate : NSObjectProtocol
```

Deprecated

Use MCBrowserViewController along with MCBrowserViewControllerDelegate from the MultipeerConnectivity framework.

## Topics

### Creating a Session for the Peer Picker

func peerPickerController(GKPeerPickerController, didSelect: GKPeerPickerConnectionType)

Tells the delegate that the user selected a connection type.

func peerPickerController(GKPeerPickerController, sessionFor: GKPeerPickerConnectionType) -> GKSession

Asks the delegate to return a session for the specified connection type.

### Responding to Connection Messages

func peerPickerController(GKPeerPickerController, didConnectPeer: String, to: GKSession)

Tells the delegate that the controller connected a peer to the session.

### Responding When the User Cancels the Connection Attempt

func peerPickerControllerDidCancel(GKPeerPickerController)

Tells the delegate that the user canceled the connection attempt.

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

protocol GKSessionDelegate

An object implements the GKSessionDelegate protocol to control the behavior of a GKSession object. The delegate is called when other visible peers change their state relative to the session. It is also called to determine whether another peer is allowed to connect to the session.

Deprecated

protocol GKTurnBasedEventHandlerDelegate

The GKTurnBasedEventHandlerDelegate protocol is implemented by an object to receive notifications events for turn-based matches. All methods are called on the main thread.

Deprecated

protocol GKVoiceChatClient

The GKVoiceChatClient protocol is implemented to control the behavior of the GKVoiceChatService object. The voice chat client has a number of responsibilities:

Deprecated

