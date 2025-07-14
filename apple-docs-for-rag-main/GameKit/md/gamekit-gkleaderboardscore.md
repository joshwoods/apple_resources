

- GameKit
-  GKLeaderboardScore 

Class

# GKLeaderboardScore

Information about a player’s score on a leaderboard.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
class GKLeaderboardScore
```

## Overview

A GKLeaderboardScore object represents a score on a leaderboard for scores you report for challenges or turn-based games.

When you create a GKLeaderboardScore object, set the `leaderboardID` property to the associated leaderboard, the `player` property to the player who earns the score, and the `value` property to the score. Make sure the score is compatible with the score format that you configure in App Store Connect.

Then use either the report(_:withEligibleChallenges:withCompletionHandler:) or endMatchInTurn(withMatch:leaderboardScores:achievements:completionHandler:) `GKTurnBasedMatch` method to report one or more scores.

For details about the score format, see Configure leaderboards in App Store Connect Help.

## Topics

### Accessing Properties

var context: Int

An integer value that your game uses.

var leaderboardID: String

The ID that Game Center uses for the leaderboard.

var player: GKPlayer

The player who earns the score.

var value: Int

The score that the player earns.

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
- Sendable

## See Also

### Leaderboards

Encourage progress and competition with leaderboards

Let players measure their own progress and compare their skills with friends and others.

Creating recurring leaderboards

Create a leaderboard for your game that ranks player scores based on a schedule.

Adding Recurring Leaderboards to Your Game

Encourage competition in your games by adding leaderboards that have a duration and repeat.

class GKLeaderboard

A leaderboard for a game that Game Center stores.

class GKLeaderboardSet

Organizes leaderboards into logical and coherent groups.

