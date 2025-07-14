

- GameKit
-  GKScore Deprecated

Class

# GKScore

An object containing information for a score that was earned by the player.

iOS 4.1–14.0DeprecatediPadOS 4.1–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedmacOS 10.8–11.0DeprecatedtvOS 9.0–14.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–7.0Deprecated

``` source
class GKScore
```

Deprecated

Use the GKLeaderboard.Entry class instead.

## Overview

Important

Your game must authenticate a local player before you can use any Game Center classes. If there is no authenticated player, your game receives a GKError.Code.notAuthenticated error. For more information, see Authenticating a player.

Your game creates `GKScore` objects to post scores to a leaderboard on Game Center. When your game retrieves score information from a leaderboard, those scores are returned as `GKScore` objects.

Scores and leaderboards work together to help you create a better game. Whenever a new `GKScore` object is created, it is associated with a leaderboard. You must ensure that the score being sent to a leaderboard is compatible with the leaderboard scoring format set in App Store Connect. See Leaderboards and Leaderboard Sets for information on how to create a leaderboard in App Store Connect.

To report a score to Game Center, your game allocates and initializes a new object, sets the value property to the score the player earned, and then calls the report(completionHandler:) method. The mechanism your game uses to calculate scores is up to you to design; scores are only compared within your game.

## Topics

### Reporting a New Score

class func report([GKLeaderboardScore], withEligibleChallenges: [GKChallenge], withCompletionHandler: (((any Error)?) -> Void)?)

Submits a list of scores and all eligible challenges.

class func report([GKScore], withCompletionHandler: (((any Error)?) -> Void)?)

Reports a list of scores to Game Center

class func report([GKScore], withEligibleChallenges: [GKChallenge], withCompletionHandler: (((any Error)?) -> Void)?)

Submits a list of scores and all eligible challenges.

### Issuing a Score Challenge

func challengeComposeController(withMessage: String?, players: [GKPlayer]?, completion: GKChallengeComposeHandler?) -> UIViewController

Provides a challenge compose view controller with preselected player identifiers and a preformatted, player-editable message.

typealias GKChallengeComposeHandler

A completion block that provides information about the player who issues a challenge and the players who receive it.

func challengeComposeController(withMessage: String?, players: [GKPlayer]?, completionHandler: GKChallengeComposeCompletionBlock?) -> UIViewController

Provides a challenge compose view controller with pre-selected player identifiers and a preformatted, player-editable message.

func challengeComposeController(withPlayers: [String]?, message: String?, completionHandler: GKChallengeComposeCompletionBlock?) -> UIViewController?

Provides a challenge compose view controller with pre-selected player identifiers and a preformatted, player-editable message.

### Deprecated Methods and Properties

var category: String?

The leaderboard that this score belongs to.

var context: UInt64

An integer value used by your game.

var date: Date

The date and time when the score was earned.

var formattedValue: String?

Returns the player’s score as a localized string.

var leaderboardIdentifier: String

The identifier for the leaderboard.

var player: GKPlayer

The player who earned the score.

var rank: Int

The position of the score in the results of a leaderboard search.

var value: Int64

The score earned by the player.

var shouldSetDefaultLeaderboard: Bool

A Boolean value that indicates whether this score should also update the default leaderboard.

init(leaderboardIdentifier: String)

Returns an initialized score object using the local player and the current date.

init(leaderboardIdentifier: String, player: GKPlayer)

Returns an initialized score object for the specified leaderboard and player.

init(category: String?)

Returns an initialized score object.

init?(leaderboardIdentifier: String, forPlayer: String)

Returns an initialized score object for the specified leaderboard and player.

func issueChallenge(toPlayers: [String]?, message: String?)

Issues a score challenge to a set of players.

var playerID: String?

The player identifier for the player that earned the score.

func report(completionHandler: (((any Error)?) -> Void)?)

Reports a score to Game Center.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

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

