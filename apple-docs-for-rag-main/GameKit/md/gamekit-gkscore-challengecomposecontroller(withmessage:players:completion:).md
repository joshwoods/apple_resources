

- GameKit
- GKScore
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

The challenge that GameKit sends to other players.

`players`  

The players to invite to the challenge.

`completionHandler`  

A block that GameKit calls after it displays the view controller.

## See Also

### Issuing a Score Challenge

typealias GKChallengeComposeHandler

A completion block that provides information about the player who issues a challenge and the players who receive it.

func challengeComposeController(withMessage: String?, players: [GKPlayer]?, completionHandler: GKChallengeComposeCompletionBlock?) -> UIViewController

Provides a challenge compose view controller with pre-selected player identifiers and a preformatted, player-editable message.

Deprecated

func challengeComposeController(withPlayers: [String]?, message: String?, completionHandler: GKChallengeComposeCompletionBlock?) -> UIViewController?

Provides a challenge compose view controller with pre-selected player identifiers and a preformatted, player-editable message.

Deprecated

