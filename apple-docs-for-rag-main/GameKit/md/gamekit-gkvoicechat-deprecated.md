

- GameKit
-  GKVoiceChat Deprecated

Class

# GKVoiceChat

A voice channel that allows players to speak with each other in a multiplayer game.

iOS 4.1–18.0DeprecatediPadOS 4.1–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.8–15.0DeprecatedtvOS 9.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
class GKVoiceChat
```

Deprecated

Use SharePlay instead. See Enable the local player to choose other players and startGroupActivity(playerHandler:).

## Mentioned in 

Adding voice chat to multiplayer games

## Overview

GameKit provides the underlying mechanism to implement voice chat between players in a multiplayer game. It’s your responsibility to provide player controls and display feedback during the chat.

First, configure voice chat by adding the NSMicrophoneUsageDescription key to the Information Property List and creating an audio session. Then, create a `GKVoiceChat` object using the `GKMatch` voiceChat(withName:) method passing a string that identifies the voice channel. Use the start() method to connect players to the channel. Use the isActive property to activate the microphone or switch the microphone between channels.

Provide a handler using the playerVoiceChatStateDidChangeHandler property to update the interface when a player connects, speaks, or disconnects from a chat. You can also add controls that mute and set the volume using the setPlayer(_:muted:) method and volume property.

Note that if there’s insufficient bandwidth over Wi-Fi to maintain a voice chat, GameKit may disconnect players from the channel or disband a channel.

## Topics

### Determining Whether Voice Chat Is Available

class func isVoIPAllowed() -> Bool

Returns whether voice chat is available on the device.

### Starting and Stopping Voice Chat

func start()

Starts communication with other players in a channel.

func stop()

Ends communication with other players in a channel.

var isActive: Bool

A Boolean value that indicates whether the channel is sampling the microphone.

### Receiving Updates About Other Participants

var playerVoiceChatStateDidChangeHandler: (GKPlayer, GKVoiceChat.PlayerState) -> Void

A method that handles when a player’s voice chat changes state.

enum PlayerState

The state of a player in a voice chat.

### Controlling Chat Volume

func setPlayer(GKPlayer, muted: Bool)

Mutes a player in the chat, including the local player.

var volume: Float

The volume level for the channel.

### Accessing Properties

var name: String

The name of the voice chat channel.

var players: [GKPlayer]

The players connected to the channel.

### Deprecated Methods and Properties

var playerIDs: [String]?

An array of strings containing the player identifiers for the players connected to the channel.

var playerStateUpdateHandler: (String, GKVoiceChat.PlayerState) -> Void

Handles when a player in the chat changes state.

func setMute(Bool, forPlayer: String)

Mutes a player in a voice chat.

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

class GKVoiceChatService

The GKVoiceChatService class allows your application to connect two iOS devices into a voice chat.

Deprecated

