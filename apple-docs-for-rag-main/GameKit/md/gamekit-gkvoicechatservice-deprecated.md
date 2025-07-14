

- GameKit
-  GKVoiceChatService Deprecated

Class

# GKVoiceChatService

The GKVoiceChatService class allows your application to connect two iOS devices into a voice chat.

visionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

``` source
class GKVoiceChatService
```

Deprecated

Use SharePlay instead

## Overview

Before you can use voice chat, your application must configure an audio session that allows for both play and recording (kAudioSessionCategory_PlayAndRecord). For more information on audio sessions, see Audio Session Programming Guide.

The voice chat service uses a client implemented by your application to find and connect to other participants. Each participant in the chat is identified by a unique *participant identifier* string. The client provides a participant identifier for the local user and translates other participant identifiers into connections to other users. The format and mechanism used to translate participant identifiers into network connections is defined by the client.

Your application can configure the voice chat service to control the volume level of both local and remote participants and to detect when someone is speaking.

To use the voice chat service, your application retrieves the default service and attaches a client to it, then either connects to another participant or waits for them to start a connection.

## Topics

### Determining Whether Voice Chat Is Available

class func isVoIPAllowed() -> Bool

Returns whether voice chat is allowed to be used on the device.

### Getting the Shared Voice Chat Service

class func `default`() -> GKVoiceChatService!

Retrieves the singleton chat service.

### Setting the Client

var client: (any GKVoiceChatClient)!

An object that the voice chat service uses to communicate with remote participants.

### Establishing a Voice Chat

func startVoiceChat(withParticipantID: String!) throws

Sends a request to another participant to join the voice chat.

### Adjusting Audio Properties

var isMicrophoneMuted: Bool

A Boolean value that determines whether the user’s microphone is muted.

var remoteParticipantVolume: Float

A float that scales the volume of all remote participants.

### Monitoring the Audio Level

var isInputMeteringEnabled: Bool

A Boolean value that indicates whether the microphone’s sound level is being monitored.

var inputMeterLevel: Float

The volume, in decibels (db), being received by the microphone.

var isOutputMeteringEnabled: Bool

A Boolean value that indicates whether the voice level of remote participants is monitored.

var outputMeterLevel: Float

The volume, in decibels (db), being received from all other participants.

### Ending a Voice Chat

func stopVoiceChat(withParticipantID: String!)

Ends a previously established voice chat.

### Methods Called by the Client

func acceptCallID(Int) throws

Accepts a request from a remote user to establish a voice chat.

func denyCallID(Int)

Rejects a request to establish a voice chat.

func receivedData(Data!, fromParticipantID: String!)

Called by the client to deliver new data received from a remote participant.

func receivedRealTime(Data!, fromParticipantID: String!)

Called by the client to deliver voice data received from a remote participant..

### Constants

Voice Chat Service Error Domain

The GKVoiceChatService error domain.

enum Code

Error codes for the voice chat service error domain.

struct GKVoiceChatServiceError

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

