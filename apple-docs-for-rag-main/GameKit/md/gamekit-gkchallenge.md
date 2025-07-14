

- GameKit
-  GKChallenge 

Class

# GKChallenge

A challenge issued by the local player to another player.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
class GKChallenge
```

## Overview

Players can use Game Center to challenge other players to beat their scores and achievements that they earn in your game. When a player issues a challenge to another player, Game Center sends a push notification to the other player. That player can then accept or refuse the challenge. If the player accepts the challenge, Game Center adds the challenge to the player’s list of challenges. Later, if the player beats the challenge, Game Center notifies both players.

Game Center supports two kinds of challenges:

score challenge (GKScoreChallenge)  
When a player challenges another player to beat their leaderboard score. When the player beats the score, Game Center issues a new score challenge to the player who initiated the challenge and continues issuing challenges between the players until a player refuses the challenge.

achievement challenge (GKAchievementChallenge)  
When a player challenges another player to earn an achievement. This challenge ends when the player earns the achievement.

You never subclass the GKChallenge class directly. However, you can subclass GKScoreChallenge or GKAchievementChallenge to create specific kinds of challenges.

### Enable Challenges

You must enable challenges for your game in App Store Connect before you can use the challenges features. For details, see Enable challenges in App Store Connect Help.

### Load and Issue Challenges

You can load the challenges issued by the local player using the loadReceivedChallenges(completionHandler:) class method. You can issue challenges with the player’s permission using the challengeComposeController(withMessage:players:completion:) method in the GKLeaderboard.Entry, GKScore, or GKAchievement class.

## Topics

### Retrieving the List of Challenges to the Local Player

class func loadReceivedChallenges(completionHandler: (([GKChallenge]?, (any Error)?) -> Void)?)

Loads the list of outstanding challenges.

### Examining Details about a Challenge

var issuingPlayer: GKPlayer?

The player who issues the challenge.

var receivingPlayer: GKPlayer?

The player who receives the challenge.

var message: String?

A text message that describes the challenge.

var state: GKChallengeState

The current state of the challenge.

enum GKChallengeState

The state of a challenge.

var issueDate: Date

The date the player issued the challenge.

var completionDate: Date?

The date the challenged player completed the challenge.

### Declining a Challenge

func decline()

Declines a challenge that another player issues to the local player.

### Deprecated symbols

var issuingPlayerID: String?

The player who issues the challenge.

Deprecated

var receivingPlayerID: String?

The player who receives the challenge.

Deprecated

typealias GKChallengeComposeCompletionBlock

A completion block that provides information about the player who issues a challenge and the players who receive it.

Deprecated

## Relationships

### Inherits From

- NSObject

### Inherited By

- GKAchievementChallenge
- GKScoreChallenge

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

### Challenges

class GKScoreChallenge

A type of challenge where a player must beat the leaderboard score of another player.

class GKAchievementChallenge

A type of challenge where a player must earn another player’s achievement.

protocol GKChallengeListener

An object that responds to challenge events.

GKShowChallengeBanners

A Boolean value that indicates whether GameKit can display challenge banners in a game.

