

- GameKit
- GKLeaderboard
- GKLeaderboard.Entry
-  challengeComposeController(withMessage:players:completion:) 

Instance Method

# challengeComposeController(withMessage:players:completion:)

Provides a challenge compose view controller with preselected player identifiers and a preformatted, player-editable message.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
func challengeComposeController(
    withMessage message: String?,
    players: [GKPlayer]?,
    completion completionHandler: GKChallengeComposeHandler? = nil
) -> UIViewController
```

**macOS**

``` source
func challengeComposeController(
    withMessage message: String?,
    players: [GKPlayer]?,
    completion completionHandler: GKChallengeComposeHandler? = nil
) -> NSViewController
```

## Parameters 

`message`  

The preformatted, player-editable message that GameKit sends to the players in the challenge.

`players`  

The players to invite to the challenge.

`completionHandler`  

A block that GameKit calls after it displays the view controller.

## Return Value

A UIViewController containing the player identifiers and a player-editable message.

## Discussion

GameKit presents the returned view controller modally on the top view controller. After GameKit displays the view controller and the player sends or cancels the challenge, GameKit calls the completion handler block on the main thread.

## See Also

### Presenting Challenges

typealias GKChallengeComposeHandler

A completion block that provides information about the player who issues a challenge and the players who receive it.

func challengeComposeController(withMessage: String?, players: [GKPlayer]?, completionHandler: GKChallengeComposeCompletionBlock?) -> UIViewController

Provides a challenge compose view controller with preselected player identifiers and a preformatted, player-editable message.

Deprecated

