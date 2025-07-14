

- GameKit
- GKTurnBasedMatch
-  sendReminder(to:localizableMessageKey:arguments:completionHandler:) 

Instance Method

# sendReminder(to:localizableMessageKey:arguments:completionHandler:)

Sends a reminder from one participant to a specific set of other participants.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
func sendReminder(
    to participants: [GKTurnBasedParticipant],
    localizableMessageKey key: String,
    arguments: [String],
    completionHandler: (((any Error)?) -> Void)? = nil
)
```

``` source
func sendReminder(
    to participants: [GKTurnBasedParticipant],
    localizableMessageKey key: String,
    arguments: [String]
) async throws
```

## Parameters 

`participants`  

The participants who Game Center sends the reminder to.

`key`  

The identifier for looking up the translated string in the default `Localized.strings` file. If you use a formatted string with specifiers, provide the arguments.

`arguments`  

A list of arguments to substitute into the localized string if it’s formatted and contains specifiers.

`completionHandler`  

The block that GameKit calls when it completes the request.

The block receives the following parameter:

*error*  
Describes an error if it occurs, or `nil` if the operation completes.

## Mentioned in 

Sending messages to players in turn-based games

## Discussion

Use this method to send a localized message to participants of a turn-based event or exchange request that needs their attention.

If your game isn’t running on recipient devices, the notification containing the localized message appears immediately at the top of the screen. When the participant taps or clicks the notification, GameKit launches your game and invokes the `GKTurnBasedEventListener` player(_:receivedTurnEventFor:didBecomeActive:) protocol method.

GameKit uses the recipient’s language and region to localize the message. If the recipient doesn’t have the game installed on their device, GameKit uses the sender’s localization settings instead. See Sending messages to players in turn-based games.

## See Also

### Sending Messages Between Participants

var message: String?

A message from the current participant to all other participants when you end a turn, forfeit a match, or end a match.

func setLocalizableMessageWithKey(String, arguments: [String]?)

Sends a localized message from the current participant to all other participants when you end a turn, forfeit a match, or end a match.

