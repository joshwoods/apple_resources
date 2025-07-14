

- GameKit
- GKScore
-  challengeComposeController(withPlayers:message:completionHandler:) Deprecated

Instance Method

# challengeComposeController(withPlayers:message:completionHandler:)

Provides a challenge compose view controller with pre-selected player identifiers and a preformatted, player-editable message.

iOS 7.0–8.0DeprecatediPadOS 7.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOS 9.0–17.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func challengeComposeController(
    withPlayers playerIDs: [String]?,
    message: String?,
    completionHandler: GKChallengeComposeCompletionBlock? = nil
) -> UIViewController?
```

## Parameters 

`playerIDs`  

An array of NSString objects that contains the player identifiers that the challenge is to be sent to.

`message`  

The preformatted, player-editable message that is being sent to other players.

`completionHandler`  

A block to be called after the view controller has been displayed. Contains the reason the handler was called and all player identifiers that the challenge was sent to.

## Return Value

A UIViewController view containing the player identifiers and a player-editable message.

## Discussion

The view controller returned is presented modally from the top view controller. After the view controller is displayed and the player sends or cancels the challenge, the completion handler block is called.

When this method is called, it creates a new background task to handle the request. The method then returns control to your game. Later, when the task is complete, GameKit calls your completion handler. The completion handler is always called on the main thread.

## See Also

### Issuing a Score Challenge

func challengeComposeController(withMessage: String?, players: [GKPlayer]?, completion: GKChallengeComposeHandler?) -> UIViewController

Provides a challenge compose view controller with preselected player identifiers and a preformatted, player-editable message.

typealias GKChallengeComposeHandler

A completion block that provides information about the player who issues a challenge and the players who receive it.

func challengeComposeController(withMessage: String?, players: [GKPlayer]?, completionHandler: GKChallengeComposeCompletionBlock?) -> UIViewController

Provides a challenge compose view controller with pre-selected player identifiers and a preformatted, player-editable message.

Deprecated

