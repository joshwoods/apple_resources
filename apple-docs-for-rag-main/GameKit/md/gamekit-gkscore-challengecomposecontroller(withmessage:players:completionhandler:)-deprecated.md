

- GameKit
- GKScore
-  challengeComposeController(withMessage:players:completionHandler:) Deprecated

Instance Method

# challengeComposeController(withMessage:players:completionHandler:)

Provides a challenge compose view controller with pre-selected player identifiers and a preformatted, player-editable message.

iOS 8.0–17.0DeprecatediPadOS 8.0–17.0DeprecatedMac Catalyst 13.1–17.0DeprecatedmacOS 10.10–14.0DeprecatedtvOS 9.0–17.0DeprecatedvisionOS 1.0–1.0Deprecated

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
func challengeComposeController(
    withMessage message: String?,
    players: [GKPlayer]?,
    completionHandler: GKChallengeComposeCompletionBlock? = nil
) -> UIViewController
```

**macOS**

``` source
func challengeComposeController(
    withMessage message: String?,
    players: [GKPlayer]?,
    completionHandler: GKChallengeComposeCompletionBlock? = nil
) -> NSViewController
```

## Parameters 

`message`  

The preformatted, player-editable message that is being sent to other players.

`players`  

An array of GKPlayer objects that contains the player identifiers that the challenge is to be sent to.

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

func challengeComposeController(withPlayers: [String]?, message: String?, completionHandler: GKChallengeComposeCompletionBlock?) -> UIViewController?

Provides a challenge compose view controller with pre-selected player identifiers and a preformatted, player-editable message.

Deprecated

