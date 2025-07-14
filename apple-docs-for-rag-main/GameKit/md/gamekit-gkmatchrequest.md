

- GameKit
-  GKMatchRequest 

Class

# GKMatchRequest

An object that encapsulates the parameters to create a real-time or turn-based match.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
class GKMatchRequest
```

## Mentioned in 

Finding players using matchmaking rules

Finding multiple players for a game

Starting turn-based matches and passing turns between players

Finding players with similar skill levels

Assigning players to teams using rules

## Overview

To request a match, set the properties of the match request, such as the number of players, the invitation message, and whether to use automatch to fill the player slots. You’re required to set the minimum and maximum number of players allowed in the match. Then, pass the match request to the appropriate class, depending on the type of game and whether you implement your own user interface.

To use the matchmaking user interface that GameKit provides, pass the match request to the GKMatchmakerViewController class for real-time games, or the GKTurnBasedMatchmakerViewController class for turn-based games. GameKit sends messages to the delegates of these classes when players receive and accept invitations to the match.

If you implement your own interface for finding players, pass the match request to the GKMatchmaker class for real-time games, or the GKTurnBasedMatch class for turn-based games. If the player selects the other players to invite in your interface, set the recipients, the inviteMessage, and the recipientResponseHandler properties before creating the match.

### Matchmaking using rules

You can refine the match results and reduce player wait times by configuring matchmaking before you present an interface. You can either find players using matchmaking rules you set up on the server, or find players from a subset of players you specify in the game.

To use matchmaking rules, set the queueName property to the queue name that you configure in App Store Connect. Optionally, set properties and recipientProperties to game-specific criteria. Players in the recipientProperties property need to also be in the recipients property — that is, be a recipient of an invitation. When using matchmaking rules, Game Center ignores the subset that you specify using the playerGroup and playerAttributes properties.

If you set the request’s minPlayers and maxPlayers properties, use values that are in the rule set’s player range. Otherwise, the default values for these properties are the rule set’s `minPlayers` and `maxPlayers` fields (see Create a rule set).

If you don’t use matchmaking rules, you can restrict finding players to a subset of players. Set the queueName property to `nil`, and set the playerGroup and playerAttributes properties to specify the subset. Then matchmaking ignores the rules-based properties and recipientProperties properties.

For more information, see Finding players using matchmaking rules.

Important

Matchmaking rules are only available for peer-to-peer (GKMatchType.turnBased) and hosted (GKMatchType.hosted) match requests.

## Topics

### Restricting the number of players

class func maxPlayersAllowedForMatch(of: GKMatchType) -> Int

Returns the maximum number of players allowed in the match request for a given match type.

enum GKMatchType

The kind of match managed by Game Center.

var minPlayers: Int

The minimum number of players that can join the match.

var maxPlayers: Int

The maximum number of players that can join the match.

var defaultNumberOfPlayers: Int

The default number of players for the match.

### Inviting players

var inviteMessage: String?

The message sent to other players when the local player invites them to join a match.

var recipients: [GKPlayer]?

The players to invite to the match.

var recipientResponseHandler: ((GKPlayer, GKInviteRecipientResponse) -> Void)?

A method that handles when a player responds to an invitation to join a match.

enum GKInviteRecipientResponse

A player’s response to an invitation to join a match.

### Matching players using rules

var queueName: String?

The name of the queue that Game Center places the match request in.

var properties: [String : Any]?

The criteria for the local player that Game Center uses to find other players when using matchmaking rules.

var recipientProperties: [GKPlayer : [String : Any]]?

The criteria for recipients of the match request that Game Center uses to find other players when using matchmaking rules.

### Matching specific players

var playerGroup: Int

A number identifying a subset of players invited to join a match.

var playerAttributes: UInt32

A mask that specifies the role that the local player would like to play in the game.

### Deprecated methods and properties

var inviteeResponseHandler: ((String, GKInviteeResponse) -> Void)?

Handles when a player responds to an invitation.

Deprecated

typealias GKInviteeResponse

Possible responses from an invitation to a remote player.

Deprecated

var playersToInvite: [String]?

A list of player identifiers for players to invite to the match.

Deprecated

var restrictToAutomatch: Bool

A Boolean value that determines whether a game uses automatch to find players or the local player invites players.

Deprecated

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

### Real-time games

Creating real-time games

Develop games where multiple players interact in real time.

Finding multiple players for a game

Discover and invite other players to participate in a real-time game.

Exchanging data between players in real-time games

Send data between players in a real-time multiplayer game.

Adding voice chat to multiplayer games

Enable players to voice chat with all, or groups of, players in a multiplayer game.

Matchmaking rules

Game Center applies different type of rules you create in a particular order to find the best matches.

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

