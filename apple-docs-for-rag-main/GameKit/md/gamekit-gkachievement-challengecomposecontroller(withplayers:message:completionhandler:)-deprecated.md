

- GameKit
- GKAchievement
-  challengeComposeController(withPlayers:message:completionHandler:) Deprecated

Instance Method

# challengeComposeController(withPlayers:message:completionHandler:)

Provides a challenge compose view controller with preselected player identifiers and a message.

iOS 7.0–8.0DeprecatediPadOS 7.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOS 9.0–17.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func challengeComposeController(
    withPlayers playerIDs: [String]?,
    message: String?,
    completionHandler: GKChallengeComposeCompletionBlock? = nil
) -> UIViewController?
```

Deprecated

Use the challengeComposeController(withMessage:players:completion:) method instead.

## Parameters 

`playerIDs`  

An array of `NSString` objects that contains the player identifiers that the challenge is to be sent to.

`message`  

The message that is sent to other players. This message can be edited by the player.

`completionHandler`  

A block to be called after the view controller has been displayed. Contains the reason the handler was called and all player identifiers that the challenge was sent to.

## Return Value

A `UIViewController` view that contains the player identifiers and the challenge message.

## Discussion

When this method is called, it creates a new background task to handle the request. The method then returns control to your game. Later, when the task is complete, Game Kit calls your completion handler. The completion handler is always called on the main thread.

The view controller returned is presented modally from the top view controller. After the view controller is displayed and the player sends or cancels the challenge, the completion handler block is called.

## See Also

### Issuing Achievement Challenges

func selectChallengeablePlayers([GKPlayer], withCompletionHandler: (([GKPlayer]?, (any Error)?) -> Void)?)

Finds the subset of players who can earn an achievement.

func challengeComposeController(withMessage: String?, players: [GKPlayer], completion: GKChallengeComposeHandler?) -> UIViewController

Provides a view controller that you present to the player to issue an achievement challenge.

typealias GKChallengeComposeHandler

A completion block that provides information about the player who issues a challenge and the players who receive it.

func challengeComposeController(withMessage: String?, players: [GKPlayer], completionHandler: GKChallengeComposeCompletionBlock?) -> UIViewController

Provides a view controller that you present to the player to issue an achievement challenge.

Deprecated

