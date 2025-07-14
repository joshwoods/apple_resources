

- GameKit
-  Sending messages to players in turn-based games 

Article

# Sending messages to players in turn-based games

Notify players of match events by sending messages and game data.

## Overview

GameKit provides several APIs for you to communicate events and send messages in your turn-based games. You can include a message and custom game data in the GKTurnBasedMatch object passed between active participants. You can also send a notification to other participants when they’re not running your game.

To send other types of data between players when they’re not taking their turn, see the GKTurnBasedExchange class.

Important

The code listings in this article use GameKit asynchronous methods that you invoke from an `async` method or within a `Task` structure. For details on asynchronous flows, see Concurrency.

### Pass messages from the current participant

You can send localized or non-localized messages from the current participant to others in a turn-based match using the GKTurnBasedMatch object. If the game isn’t running or is in the background, the message you provide appears immediately at the top of the screen as a notification. If the game is in the foreground, get the message from the match object GameKit passes to participants and display it in your own interface.

Before you perform an action such as ending a turn, set the message property of the match object. Alternatively, set a message that GameKit localizes using the receiving participant’s language and region settings using the setLocalizableMessageWithKey(_:arguments:) method.

```
match.message = "We're all counting on you!"
try await match.endTurn(withNextParticipants: nextParticipants, turnTimeout: GKTurnTimeoutDefault, match: gameData)
```

If a participant taps the notification when it appears, GameKit launches the game or brings it to the foreground. GameKit invokes the `GKTurnBasedEventListener` player(_:receivedTurnEventFor:didBecomeActive:) protocol method passing true as the active parameter. Implement this method to join the match. For more information on handling turn-based events, see Starting turn-based matches and passing turns between players.

If the game is in the foreground, GameKit invokes this method but passes false as the active parameter. You can then present the message in your own interface by getting the message from the match object using the message property.

To localize a message, add the key you pass to the setLocalizableMessageWithKey(_:arguments:) method and a placeholder translation to a `.strings` file in your project (for example, the default `Localizable.strings` file). For more information on adapting your game for different languages and regions, see Localization.

### Send messages from any participant

Send a localized message from any participant to others using a Game Center notification. For example, send a reminder to the current participant from another participant who is waiting for them to take their turn. GameKit sends the reminder to the participants as a push notification that doesn’t interrupt their gameplay. The notification only appears when the game isn’t running — it doesn’t appear if the participant runs the game in either the foreground or background.

To display the GameKit notification:

1.  Invoke the `GKTurnBasedMatch` sendReminder(to:localizableMessageKey:arguments:completionHandler:) method passing the participants and a localized message key:

```
// Create an array that contains the current participant.
let participants = match.participants.filter {
    $0 == match.currentParticipant
}

// Send a reminder to the current participant.
try await match.sendReminder(to: participants, localizableMessageKey: "It's your turn to play.", arguments: [])
```

2.  Add the localized message key and placeholder translation to a `.strings` file in your project. If necessary, add a `.strings` file (for example, the default `Localizable.strings` file) to your project and make it localizable. For the Xcode steps, see Adding resources to localizations and `Editing XLIFF and strings files`.

```
"It's your turn to play." = "It's your turn to play.";
```

When the player taps the notification, GameKit invokes the `GKTurnBasedEventListener` player(_:receivedTurnEventFor:didBecomeActive:) protocol method passing true as the active parameter. Implement this method to join the existing match. For more information on handling turn-based events, see Starting turn-based matches and passing turns between players.

Note

If you exceed the system’s 10-minute limit for the frequency of sending reminders, a `GKServerTurnBasedMaxSessionOtherError` error occurs.

## See Also

### Turn-based games

Creating turn-based games

Develop games where multiple players take turns and can exchange data while waiting for their turn.

Starting turn-based matches and passing turns between players

Let Game Center store and forward match data between players in a turn-based game.

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

