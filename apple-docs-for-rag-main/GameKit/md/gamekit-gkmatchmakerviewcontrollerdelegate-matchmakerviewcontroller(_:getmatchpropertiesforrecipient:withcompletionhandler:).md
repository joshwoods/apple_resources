

- GameKit
- GKMatchmakerViewControllerDelegate
-  matchmakerViewController(\_:getMatchPropertiesForRecipient:withCompletionHandler:) 

Instance Method

# matchmakerViewController(\_:getMatchPropertiesForRecipient:withCompletionHandler:)

Returns the properties for another player that the local player invites using the view controller interface.

iOS 17.2+iPadOS 17.2+Mac Catalyst 17.2+macOS 14.2+tvOS 17.2+visionOS 1.1+

``` source
optional func matchmakerViewController(
    _ viewController: GKMatchmakerViewController,
    getMatchPropertiesForRecipient recipient: GKPlayer,
    withCompletionHandler completionHandler: @escaping ([String : Any]) -> Void
)
```

``` source
optional func matchmakerViewController(
    _ viewController: GKMatchmakerViewController,
    getMatchPropertiesForRecipient recipient: GKPlayer
) async -> [String : Any]
```

## Parameters 

`viewController`  

The view controller that finds players for the match.

`recipient`  

A player to invite to the match.

`completionHandler`  

The block that this method calls when it completes the request.

The block receives the following parameter:

`recipientProperties`  
The properties for `recipient` that the local player invites to the match.

## Mentioned in 

Finding players using matchmaking rules

## Discussion

Implement this method if you can provide properties for the recipients of this match request to better fine tune the Game Center matchmaking using rules. For more information, see Matchmaking rules.

