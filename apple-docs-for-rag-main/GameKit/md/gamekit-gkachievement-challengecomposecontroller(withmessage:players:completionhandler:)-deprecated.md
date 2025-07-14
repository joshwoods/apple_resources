

- GameKit
- GKAchievement
-  challengeComposeController(withMessage:players:completionHandler:) Deprecated

Instance Method

# challengeComposeController(withMessage:players:completionHandler:)

Provides a view controller that you present to the player to issue an achievement challenge.

iOS 8.0–17.0DeprecatediPadOS 8.0–17.0DeprecatedMac Catalyst 13.1–17.0DeprecatedmacOS 10.10–14.0DeprecatedtvOS 9.0–17.0DeprecatedvisionOS 1.0–1.0Deprecated

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
func challengeComposeController(
    withMessage message: String?,
    players: [GKPlayer],
    completionHandler: GKChallengeComposeCompletionBlock? = nil
) -> UIViewController
```

**macOS**

``` source
func challengeComposeController(
    withMessage message: String?,
    players: [GKPlayer],
    completionHandler: GKChallengeComposeCompletionBlock? = nil
) -> NSViewController
```

Deprecated

Use the challengeComposeController(withMessage:players:completion:) method instead.

## Parameters 

`message`  

The challenge message which the player can edit before GameKit sends it to other players.

`players`  

The players that the challenge should be sent to.

`completionHandler`  

A block that GameKit calls after it displays the view controller.

## Return Value

A view controller that contains the player identifiers and the challenge message.

## Discussion

This method presents the view controller modally from the top view controller. GameKit calls the completion handler block after it displays the view controller and the player sends or cancels the challenge.

## See Also

### Issuing Achievement Challenges

func selectChallengeablePlayers([GKPlayer], withCompletionHandler: (([GKPlayer]?, (any Error)?) -> Void)?)

Finds the subset of players who can earn an achievement.

func challengeComposeController(withMessage: String?, players: [GKPlayer], completion: GKChallengeComposeHandler?) -> UIViewController

Provides a view controller that you present to the player to issue an achievement challenge.

typealias GKChallengeComposeHandler

A completion block that provides information about the player who issues a challenge and the players who receive it.

func challengeComposeController(withPlayers: [String]?, message: String?, completionHandler: GKChallengeComposeCompletionBlock?) -> UIViewController?

Provides a challenge compose view controller with preselected player identifiers and a message.

Deprecated

