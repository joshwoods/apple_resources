

- GameKit
-  GKChallengeListener 

Protocol

# GKChallengeListener

An object that responds to challenge events.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
protocol GKChallengeListener : NSObjectProtocol
```

## Overview

Your game can ignore a challenge, start up in a specific state so the local player can respond to a challenge, or notify the challenger when the local player completes a challenge.

Don’t implement GKChallengeListener directly; instead use GKLocalPlayerListener. The GKLocalPlayerListener protocol inherits methods from GKChallengeListener, GKInviteEventListener, GKSavedGameListener, and GKTurnBasedEventListener in order to handle multiple events.

## Topics

### Responding to a Challenge

func player(GKPlayer, didReceive: GKChallenge)

Handles when the local player issues a challenge but the other player doesn’t want to respond immediately.

func player(GKPlayer, wantsToPlay: GKChallenge)

Handles when the local player issues a challenge and the other player accepts.

### Completing a Challenge

func player(GKPlayer, didComplete: GKChallenge, issuedByFriend: GKPlayer)

Handles when the local player completes a challenge that a friend issues.

func player(GKPlayer, issuedChallengeWasCompleted: GKChallenge, byFriend: GKPlayer)

Handles when a friend completes a challenge that the local player issues.

## Relationships

### Inherits From

- NSObjectProtocol

### Inherited By

- GKLocalPlayerListener

## See Also

### Challenges

class GKChallenge

A challenge issued by the local player to another player.

class GKScoreChallenge

A type of challenge where a player must beat the leaderboard score of another player.

class GKAchievementChallenge

A type of challenge where a player must earn another player’s achievement.

GKShowChallengeBanners

A Boolean value that indicates whether GameKit can display challenge banners in a game.

