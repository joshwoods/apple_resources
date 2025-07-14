

- GameKit
-  Matchmaking rules 

# Matchmaking rules

Game Center applies different type of rules you create in a particular order to find the best matches.

## Overview

With matchmaking rules, you have finer control over automatch of players to fill empty slots in peer-to-peer and hosted match requests. During development, you use the matchmaking rules APIs to upload your rules to the Game Center server. You group rules into rule sets and assign the rule sets to queues. In your game code, you configure match requests to use your set of matchmaking rules by specifying a queue. Game Center applies your rules to all the match requests in the queue to fill the empty slots.

You group rules into sets for each configuration, feature, or purpose in your game and associate the rule sets with a queue. Game instances submit match requests to specific queues, and Game Center applies the corresponding rules to the match requests in that queue. The rules contain an expression that behaves like a query to filter and prioritize the requests. Game Center finds the most compatible players that meet your criteria, in a reasonable amount of time.

For more information on this feature, see Meet rule-based matchmaking in Game Center.

### The matchmaking rules algorithm

When finding players using matchmaking rules, Game Center applies four different types of rules to match requests in the queue, along with performing other steps in the algorithm. Game Center applies the expression of the rule, which is a JMESPath formatted string with some Game Center matchmaking function additions. Depending on the type of rule, Game Center evaluates the expression on two or more match requests in the queue.

Game Center performs the following steps in sequence:

- Sorts the match requests in a queue by age of the request to minimize player wait time and then applies compatible rules to pairs of requests. *Compatible rules* compare two requests and return a Boolean value that indicates whether the requests are compatible. If all the compatible rules return true, Game Center continues processing the pair. For example, requiring the app version to be 2.0 and above is a compatible rule.

- Applies the distance rules to pairs of compatible requests. *Distance rules* compare two requests and return a numeric value between `0.0` and `1.0`. Game Center uses the value to prioritize similar requests, where `0.0` is the most similar and `1.0` is the least similar. For example, requiring the geo latency between players to be low is a distance rule.

- Prioritizes compatible matches by age and distance, and generates candidate matches that have the most number of players within the range that you specify in the rule set. Sorts candidate matches by age and applies the match rules. *Match rules* apply to a set of matches and return a Boolean value that indicates whether the requests are valid matches. For example, requiring a range in skill level between `0` and `5` is a match rule.

- Generates candidate teams from combinations of candidate matches and applies the team rules, If you add rules to assign players to teams. *Team rules* apply to a set of teams containing players and return a Boolean value that indicates whether the teams satisfy a constraint. For example, ensuring that the total skill difference between teams is less than `1` is a team rule.

For more information on matchmaking rules with examples, see Finding players using matchmaking rules. For details on the matchmaking REST APIs, see Matchmaking rules in App Store Connect API.

## Topics

### Essentials

Finding players using matchmaking rules

Create a more customized and optimized gaming experience by using matchmaking rules to find players in a real-time game.

### Rules

Letting players join matches using party codes

Add a rule that lets players invite players and join matches using a shared party code.

Finding players with similar skill levels

Add a rule to find players in a range of skill levels to balance competitive gameplay.

Assigning players to teams using rules

Set criteria for assigning players to teams in your game using matchmaking rules.

Creating matchmaking rules for backward compatibility

Add matchmaking rules that support previous classic matchmaking versions of your game.

### Testing

Testing matchmaking rules

Test your matchmaking rules before you use them in your game.

Troubleshooting matchmaking rules using metrics

Investigate issues with Game Center by evaluating your matchmaking rules using metrics endpoints.

Testing rule sets with player traffic using metrics

Get metrics on a new rule set with real match requests before releasing it.

## See Also

### Related Documentation

Game Center

Manage Game Center data and configurations for your apps.

### Real-time games

Creating real-time games

Develop games where multiple players interact in real time.

Finding multiple players for a game

Discover and invite other players to participate in a real-time game.

Exchanging data between players in real-time games

Send data between players in a real-time multiplayer game.

Adding voice chat to multiplayer games

Enable players to voice chat with all, or groups of, players in a multiplayer game.

class GKMatchRequest

An object that encapsulates the parameters to create a real-time or turn-based match.

class GKMatchmaker

An object that creates matches with other players without presenting an interface to the players.

class GKMatchmakerViewController

An interface that allows a player to invite other players to a real-time game and automatch to fill any empty slots.

protocol GKInviteEventListener

A protocol that handles invite events from Game Center.

class GKInvite

An invitation to join a match sent to the local player from another player.

class GKMatch

A peer-to-peer network between a group of players that sign into Game Center.

