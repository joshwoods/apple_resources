

- GameKit
- GKLeaderboard
- GKLeaderboard.Entry
-  challengeComposeController(withMessage:players:completionHandler:) Deprecated

Instance Method

# challengeComposeController(withMessage:players:completionHandler:)

Provides a challenge compose view controller with preselected player identifiers and a preformatted, player-editable message.

iOS 14.0–17.0DeprecatediPadOS 14.0–17.0DeprecatedMac Catalyst 14.0–17.0DeprecatedmacOS 11.0–14.0DeprecatedtvOS 14.0–17.0DeprecatedvisionOS 1.0–1.0Deprecated

**macOS**

``` source
func challengeComposeController(
    withMessage message: String?,
    players: [GKPlayer]?,
    completionHandler: GKChallengeComposeCompletionBlock? = nil
) -> NSViewController
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
func challengeComposeController(
    withMessage message: String?,
    players: [GKPlayer]?,
    completionHandler: GKChallengeComposeCompletionBlock? = nil
) -> UIViewController
```

## Parameters 

`message`  

The preformatted, player-editable message that GameKit sends to the players in the challenge.

`players`  

Players to invite to the challenge.

`completionHandler`  

A block that GameKit calls after it displays the view controller.

## Return Value

A UIViewController containing the player identifiers and a player-editable message.

## Discussion

GameKit presents the returned view controller modally on the top view controller. After GameKit displays the view controller and the player sends or cancels the challenge, GameKit calls the completion handler block on the main thread.

## See Also

### Presenting Challenges

func challengeComposeController(withMessage: String?, players: [GKPlayer]?, completion: GKChallengeComposeHandler?) -> UIViewController

Provides a challenge compose view controller with preselected player identifiers and a preformatted, player-editable message.

typealias GKChallengeComposeHandler

A completion block that provides information about the player who issues a challenge and the players who receive it.

