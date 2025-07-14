

- GameKit
-  GKChallengeEventHandlerDelegate Deprecated

Protocol

# GKChallengeEventHandlerDelegate

You implement the GKChallengeEventHandlerDelegate delegate to control how challenges are displayed in your game.

macOS 10.8–10.10DeprecatedvisionOS 1.0–1.0Deprecated

``` source
protocol GKChallengeEventHandlerDelegate : NSObjectProtocol
```

Deprecated

You should instead implement the GKChallengeListener protocol and register a listener with GKLocalPlayer.

## Overview

By default, GameKit briefly displays a banner over your game when any of the following events occur:

- The local player receives a challenge.

- The local player completes a challenge.

- A remote player completes a challenge issued by the local player.

Your event handler can override or extend this behavior:

- It can prevent a banner from being displayed.

- It can be notified when a player taps in a banner.

- It can handle the events directly.

## Topics

### Detecting When a User Taps a Banner

func localPlayerDidSelect(GKChallenge!)

Called when the local player selects a challenge banner displayed by GameKit.

### Responding When a New Challenge is Received

func localPlayerDidReceive(GKChallenge!)

Called when the local player receives a new challenge.

func shouldShowBanner(forLocallyReceivedChallenge: GKChallenge!) -> Bool

Called to determine whether a banner should be shown when the local player receives a challenge.

### Responding to Challenges Completed By the Local Player

func localPlayerDidComplete(GKChallenge!)

Called when the local player completes a challenge.

func shouldShowBanner(forLocallyCompletedChallenge: GKChallenge!) -> Bool

Called to determine whether a banner should be shown when the local player completes a challenge.

### Responding to Challenges Issued by the Local Player

func remotePlayerDidComplete(GKChallenge!)

Called when a remote player completes a challenge issued by the local player.

func shouldShowBanner(forRemotelyCompletedChallenge: GKChallenge!) -> Bool

Called to determine whether a banner should be shown when a remote player completes a challenge.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Deprecated protocols

protocol GKAchievementViewControllerDelegate

An object implementing the GKAchievementViewControllerDelegate protocol is called when the user dismisses the achievements view controller. Typically, this protocol is implemented by the object in your game that originally displayed the achievements user interface.

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

protocol GKSessionDelegate

An object implements the GKSessionDelegate protocol to control the behavior of a GKSession object. The delegate is called when other visible peers change their state relative to the session. It is also called to determine whether another peer is allowed to connect to the session.

Deprecated

protocol GKTurnBasedEventHandlerDelegate

The GKTurnBasedEventHandlerDelegate protocol is implemented by an object to receive notifications events for turn-based matches. All methods are called on the main thread.

Deprecated

protocol GKVoiceChatClient

The GKVoiceChatClient protocol is implemented to control the behavior of the GKVoiceChatService object. The voice chat client has a number of responsibilities:

Deprecated

