

- GameKit
- GKAchievement
-  challengeComposeController(withMessage:players:completion:) 

Instance Method

# challengeComposeController(withMessage:players:completion:)

Provides a view controller that you present to the player to issue an achievement challenge.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
func challengeComposeController(
    withMessage message: String?,
    players: [GKPlayer],
    completion completionHandler: GKChallengeComposeHandler? = nil
) -> UIViewController
```

**macOS**

``` source
func challengeComposeController(
    withMessage message: String?,
    players: [GKPlayer],
    completion completionHandler: GKChallengeComposeHandler? = nil
) -> NSViewController
```

## Parameters 

`message`  

The challenge message, which the player can edit before GameKit sends it to other players.

`players`  

The players to invite to the challenge.

`completionHandler`  

A block that GameKit calls after it displays the view controller.

## Discussion

This method presents the view controller modally from the top view controller. GameKit calls the completion handler block after it displays the view controller and the player sends or cancels the challenge.

## See Also

### Issuing Achievement Challenges

func selectChallengeablePlayers([GKPlayer], withCompletionHandler: (([GKPlayer]?, (any Error)?) -> Void)?)

Finds the subset of players who can earn an achievement.

typealias GKChallengeComposeHandler

A completion block that provides information about the player who issues a challenge and the players who receive it.

func challengeComposeController(withMessage: String?, players: [GKPlayer], completionHandler: GKChallengeComposeCompletionBlock?) -> UIViewController

Provides a view controller that you present to the player to issue an achievement challenge.

Deprecated

func challengeComposeController(withPlayers: [String]?, message: String?, completionHandler: GKChallengeComposeCompletionBlock?) -> UIViewController?

Provides a challenge compose view controller with preselected player identifiers and a message.

Deprecated

