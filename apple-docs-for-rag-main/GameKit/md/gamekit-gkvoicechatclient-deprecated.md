

- GameKit
-  GKVoiceChatClient Deprecated

Protocol

# GKVoiceChatClient

The GKVoiceChatClient protocol is implemented to control the behavior of the GKVoiceChatService object. The voice chat client has a number of responsibilities:

visionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

``` source
protocol GKVoiceChatClient : NSObjectProtocol
```

## Overview

- Provides a network connection that the voice chat service uses to send and receive configuration data with other participants. If this network connection is shared with other application data, the client must also disambiguate between chat configuration data and application data.

- Provides a participant ID that identifies the user to remote participants in the chat.

- Defines how a remote user’s participant ID translates into a network connection to that user.

- Accepts or rejects requests from remote participants to join the voice chat.

## Topics

### Getting Information about the Participant

func participantID() -> String

Returns a string that uniquely identifies the local user.

**Required**

### Sending data to other participants

func voiceChatService(GKVoiceChatService, send: Data, toParticipantID: String)

A request for the client to send data to a participant.

**Required**

func voiceChatService(GKVoiceChatService, sendRealTime: Data, toParticipantID: String)

Asks the client to send data to a participant that must get there quickly.

### Accepting Invitations from Remote Participants

func voiceChatService(GKVoiceChatService, didReceiveInvitationFromParticipantID: String, callID: Int)

Asks the client to accept or reject an invitation from a remote participant.

### Responding to Changes in Other Participants

func voiceChatService(GKVoiceChatService, didStartWithParticipantID: String)

Received by the client when a voice chat with another participant is established.

func voiceChatService(GKVoiceChatService, didNotStartWithParticipantID: String, error: (any Error)?)

Received by the client when an attempt to establish a voice chat with another participant failed.

func voiceChatService(GKVoiceChatService, didStopWithParticipantID: String, error: (any Error)?)

Received by the client when a previously established voice chat has ended.

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

protocol GKSessionDelegate

An object implements the GKSessionDelegate protocol to control the behavior of a GKSession object. The delegate is called when other visible peers change their state relative to the session. It is also called to determine whether another peer is allowed to connect to the session.

Deprecated

protocol GKTurnBasedEventHandlerDelegate

The GKTurnBasedEventHandlerDelegate protocol is implemented by an object to receive notifications events for turn-based matches. All methods are called on the main thread.

Deprecated

