

- GameKit
-  Starting turn-based matches and passing turns between players 

Article

# Starting turn-based matches and passing turns between players

Let Game Center store and forward match data between players in a turn-based game.

## Overview

In a turn-based game, players take turns to advance gameplay, such as in chess, checkers, and similar board games.

The player who creates a match selects opponents and then takes the first turn. Then you pass the player’s turn, other game data, and the next participant to GameKit. GameKit saves the match data in Game Center, which sends the invitations to the other players. Game Center passes the turn to the next participant who accepts their invitation, until all participants reach an outcome or the match ends.

Players can participate in multiple concurrent matches that continue even after players quit a game. Game Center stores open and completed matches until the player explicitly removes them.

You manage turn-based matches through the GameKit turn-based APIs, specifically by using the GKTurnBasedMatch object that Game Center passes between participants. The match object contains the following information:

- Status of the match

- Participants and current participant

- Status and outcomes of individual participants

- A message for participants about the most recent turn

- Your game-specific data

For design guidance, see Human Interface Guidelines > Technologies > Game Center > Multiplayer.

Important

The code examples in this article use GameKit asynchronous methods that you invoke from an `async` method or within a `Task` structure. For details about asynchronous flows, see Concurrency.

### Create a match request

First, create a GKMatchRequest object that contains the parameters of your turn-based game. You can set the number of players, apply groups and attributes to filter the matches, provide an invitation message, and set other criteria.

```
let request = GKMatchRequest()
request.minPlayers = 2
request.maxPlayers = 12
```

To get the maximum number of players Game Center supports for turn-based games, pass GKMatchType.turnBased to the maxPlayersAllowedForMatch(of:) method.

### Start a turn-based match

Let players create a new match and select opponents by using the provided GameKit turn-based interface. Similar to how the process works in the real-time game interface, the player creates a match by tapping the plus button (+) in the upper-right corner. In the next few screens, the player invites players and, optionally, fills empty slots using automatch.

In your code, use the following steps to present the turn-based matchmaker interface:

1.  Create a GKTurnBasedMatchmakerViewController object by passing the GKMatchRequest object you configure in the Create a match request section above. Set its delegate to your game object that conforms to the GKTurnBasedMatchmakerViewControllerDelegate protocol.

```
let viewController = GKTurnBasedMatchmakerViewController(matchRequest: request)
viewController.turnBasedMatchmakerDelegate = self
```

2.  Configure the view controller before presenting it. Optionally, set the view controller’s matchmakingMode property to limit the use of automatch. You can also set showExistingMatches to false to remove ongoing matches that appear under Your Turn and Their Turn. Otherwise, the player can select an existing match rather than create a new one. For more information about handling existing matches, see the Open an existing turn-based match section below.

3.  Implement the GKTurnBasedMatchmakerViewControllerDelegate protocol methods to handle cancellations and errors.

4.  Then, present the turn-based matchmaker view controller to the local player.

Alternatively, create your own custom interface, and then programmatically find opponents and accept invitations using the find(for:withCompletionHandler:), acceptInvite(completionHandler:), and declineInvite(completionHandler:) methods.

### Present the gameplay interface for the player to take their turn

Before sending invitations to other players, GameKit invokes the `GKTurnBasedEventListener` player(_:receivedTurnEventFor:didBecomeActive:) protocol method for the local player to take the first turn. Later, GameKit invokes this method each time it becomes the player’s turn until the player reaches an outcome or the match ends. Implement this method to present the gameplay interface that lets the player take their turn.

To receive the GKTurnBasedEventListener callbacks, conform your game object to the GKLocalPlayerListener protocol and register it with the local player object. Register for callbacks immediately after you authenticate the local player because the system brings your game to the foreground or launches it to deliver important turn-based events. For more information about authentication, see Authenticating a player.

```
GKLocalPlayer.local.register(self)
```

Then implement the player(_:receivedTurnEventFor:didBecomeActive:) method to perform the following tasks:

1.  Retain the GKTurnBasedMatch object that GameKit passes to this method, or retain its matchID property. During gameplay, get the current match object by passing the match ID to the loadMatches(completionHandler:) class method.

2.  Update the gameplay interface by obtaining the latest game data from the match object using the matchData property. If it’s the first turn, the game data is `nil`; otherwise, it’s the game data you set when you pass the turn to the next participant.

3.  If the match status property is GKTurnBasedMatch.Status.open, configure the gameplay interface according to whose turn it is. Use the currentParticipant property to determine whether it’s the local player’s turn.

```
myTurn = GKLocalPlayer.local == match.currentParticipant?.player ? true : false
```

4.  Present your gameplay interface to the local player.

### Pass the turn to the next participant

After the player takes their turn, pass the turn to the next participant based on your game rules and logic. Implement your game to do the following:

1.  Create an array of match participants in the order you want Game Center to pass the turn. If communication fails or a participant doesn’t respond, Game Center passes the turn to the next participant in the array. Start with the participants in the GKTurnBasedMatch object. For example, exclude the current participant and other participants who, for whatever reason, aren’t active.

```
let nextParticipants = match.participants.filter (){
    ($0.status != .done) || ($0 != match.currentParticipant)
}
```

2.  Create a `Data` representation of your game data that GameKit saves and forwards to the next participant. Ensure that the size of the match data doesn’t exceed the matchDataMaximumSize property. For example, use the NSKeyedArchiver class to convert your game data to a `Data` object.

3.  Call the `GKTurnBasedMatch` endTurn(withNextParticipants:turnTimeout:match:completionHandler:) method, passing the next participant’s array, current game data, and optional timeout for the participant to take their turn.

```
try await match.endTurn(withNextParticipants: nextParticipants, turnTimeout: GKTurnTimeoutDefault, match: gameData)
```

If this is the first turn in the match, Game Center sends the invitations to other participants and then passes the turn to the next participant who accepts their invitation.

Alternatively, use the saveCurrentTurn(withMatch:completionHandler:) method to save the game data without passing the turn to the next participant. For example, save and forward game data to other participants while the player takes a more complicated, multiple-step turn.

### Accept turn-based match invitations

After the first turn, Game Center manages the status of participants for you by sending invitations and continuing to fill empty slots if you use automatch.

To join the match, a participant taps the Game Center invitation that appears on their device, and then taps the Accept button. If necessary, the system launches your game or brings it to the foreground. The player can also tap the match under New Invitations in the turn-based matchmaker interface when you present it.

When the local player joins a match, GameKit invokes the `GKTurnBasedEventListener` player(_:receivedTurnEventFor:didBecomeActive:) method. Implement this method to show the gameplay interface with the current game data, and if it’s the local player’s turn, let them take it.

Optionally, implement the player(_:didRequestMatchWithOtherPlayers:) method to notify the local player when GameKit sends the invitations.

### Display participant details

Enhance your game to show the status, name, and avatar of participants in the match when turn-based events occur. Also, be sure to update your interface when participants decline invitations or forfeit the match.

Implement the player(_:receivedTurnEventFor:didBecomeActive:) method to perform the following tasks:

1.  Get the list of all participants using the `GKTurnBasedMatch` participants property and get the participant taking their turn using the currentParticipant property.

2.  Show when participants accept their invitations and are actively playing using the `GKTurnBasedParticipant` status property. During the first turn, the status of other participants is GKTurnBasedParticipant.Status.matching because Game Center hasn’t sent the invitations. Later, the status transitions through the GKTurnBasedParticipant.Status possible values until the participant exits the match when the status becomes GKTurnBasedParticipant.Status.done.

3.  If the status property is GKTurnBasedParticipant.Status.active, display more details that become available using the player property. Display the participant’s name using the `GKPlayer` displayName property, and their avatar using the loadPhoto(for:withCompletionHandler:) method.

```
// Get the opponent's name and avatar.
opponentName = participant.player.displayName
let image = try await participant.player.loadPhoto(for: GKPlayer.PhotoSize.small)
opponentAvatar = Image(uiImage: image)
```

4.  If the status property is GKTurnBasedParticipant.Status.done, show the outcome of the participant using the matchOutcome property. For example, show whether a participant wins, loses, or forfeits a match.

### Open an existing turn-based match

A player can continue a match if they don’t forfeit it when they exit or quit your game. In the turn-based matchmaker interface, the player opens an existing match by selecting it under Your Turn or Their Turn.

When the player selects an open match, GameKit invokes the `GKTurnBasedEventListener` player(_:receivedTurnEventFor:didBecomeActive:) method. Implement this method to present the match using the current game data in the match object, and if it’s the local player’s turn, let them take it.

GameKit also invokes the player(_:receivedTurnEventFor:didBecomeActive:) method if the player selects an ended match under Completed and then clicks the View Game button on the next screen.

If the match status property is GKTurnBasedMatch.Status.ended, show the outcomes of the participants and the final game data from the match object.

If you don’t want existing matches to appear in the interface, set the view controller’s showExistingMatches to false before presenting it.

Alternatively, implement a custom interface that lets players manage existing matches. Use the `GKTurnBasedMatch` loadMatches(completionHandler:) method to load the matches from Game Center.

### Forfeit a turn-based match

A player can forfeit an open match using the turn-based matchmaker interface. The player taps the information button next to a match under Your Turn or Their Turn, and on the next screen, taps the Forfeit button in the upper-right corner. The player can also forfeit a match from the list by sliding the match to the left and tapping the Remove button. Players might also forfeit a match using a control in your gameplay interface.

GameKit invokes the `GKTurnBasedEventListener` player(_:receivedTurnEventFor:didBecomeActive:) method in the game instance of the next participant. If the player removes a match that appears under Completed, GameKit deletes the match from Game Center without notifying your game.

Implement the player(_:receivedTurnEventFor:didBecomeActive:) method to update your interface when the status of a participant changes to GKTurnBasedParticipant.Status.done. If the local player can’t continue gameplay because the number of active participants drops below the minimum number of players, end the match, as described in the next section.

To programmatically forfeit a match, call either of the following methods, depending on whether it’s the local player’s turn:

- participantQuitInTurn(with:nextParticipants:turnTimeout:match:completionHandler:)

- participantQuitOutOfTurn(with:withCompletionHandler:)

Pass GKTurnBasedMatch.Outcome.quit as the match outcome. If it’s the local player’s turn, pass an array of next participants and the current game data.

```
try await match.participantQuitInTurn(with: GKTurnBasedMatch.Outcome.quit, nextParticipants: nextParticipants, turnTimeout: GKTurnTimeoutDefault, match: gameData)
```

When a player forfeits a match, notify participants using the APIs described in Sending messages to players in turn-based games. Optionally, implement the player(_:wantsToQuitMatch:) protocol method to notify players.

### End a turn-based match

You programmatically end a match depending on your game rules and when participants reach an outcome. You can only end the match when it’s the local player’s turn.

To end a match, set the outcomes of all the participants in the match object using the matchOutcome property. For example, if the local player wins the match, set the current participant’s outcome to GKTurnBasedMatch.Outcome.won and the other participants’ outcomes to GKTurnBasedMatch.Outcome.lost.

Then call either of the following methods:

- endMatchInTurn(withMatch:completionHandler:)

- endMatchInTurn(withMatch:leaderboardScores:achievements:completionHandler:)

Optionally, pass updated game data, leaderboard scores, and achievements. If the game data doesn’t change, you can pass the existing data.

```
try await match.endMatchInTurn(withMatch: match.matchData!)
```

When a match ends, notify the participants using the APIs described in Sending messages to players in turn-based games. Optionally, implement the `GKTurnBasedEventListener` player(_:matchEnded:) protocol method to notify participants.

## See Also

### Turn-based games

Creating turn-based games

Develop games where multiple players take turns and can exchange data while waiting for their turn.

Sending messages to players in turn-based games

Notify players of match events by sending messages and game data.

Exchanging data between players in turn-based games

Add the ability for players to exchange game data and send messages while waiting for their turns.

class GKTurnBasedMatchmakerViewController

An interface that allows a player to invite other players to a turn-based match and automatch to fill any empty slots.

class GKTurnBasedMatch

An object that encapsulates the match data for games where players take turns.

class GKTurnBasedParticipant

A participant in a turn-based match.

protocol GKTurnBasedEventListener

The protocol that handles turn-based and data-exchange events between participants in a match.

class GKTurnBasedExchange

Exchange request information that participants send in a turn-based match.

class GKTurnBasedExchangeReply

Details about a recipient’s response to an exchange request.

GKGameCenterBadgingDisabled

A Boolean value indicating whether GameKit can add badges to a turn-based game icon.

