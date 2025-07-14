

- GameKit
-  GKScoreChallenge 

Class

# GKScoreChallenge

A type of challenge where a player must beat the leaderboard score of another player.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
class GKScoreChallenge
```

## Overview

To complete the challenge, the player must score an equal or better score than the other player. When the player completes the challenge, Game Center issues a new score challenge to the player who initiated the challenge and continues issuing challenges between the players until a player refuses the challenge.

## Topics

### Obtaining the score to beat

var leaderboardEntry: GKLeaderboard.Entry?

The challenger’s leaderboard score that the player must beat.

var score: GKScore?

The challenger’s leaderboard score that the player must beat.

Deprecated

## Relationships

### Inherits From

- GKChallenge

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

class GKChallenge

A challenge issued by the local player to another player.

class GKAchievementChallenge

A type of challenge where a player must earn another player’s achievement.

protocol GKChallengeListener

An object that responds to challenge events.

GKShowChallengeBanners

A Boolean value that indicates whether GameKit can display challenge banners in a game.

