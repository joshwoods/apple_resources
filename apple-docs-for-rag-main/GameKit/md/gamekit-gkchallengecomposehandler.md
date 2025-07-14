

- GameKit
-  GKChallengeComposeHandler 

Type Alias

# GKChallengeComposeHandler

A completion block that provides information about the player who issues a challenge and the players who receive it.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
typealias GKChallengeComposeHandler = (UIViewController, Bool, [GKPlayer]?) -> Void
```

**macOS**

``` source
typealias GKChallengeComposeHandler = (NSViewController, Bool, [GKPlayer]?) -> Void
```

## Parameters 

`composeController`  

The view controller for the challenge.

`didIssueChallenge`  

A Boolean value that indicates whether the player issues the challenge.

`sentPlayers`  

The players that receive the challenge.

## See Also

### Issuing Achievement Challenges

func selectChallengeablePlayers([GKPlayer], withCompletionHandler: (([GKPlayer]?, (any Error)?) -> Void)?)

Finds the subset of players who can earn an achievement.

func challengeComposeController(withMessage: String?, players: [GKPlayer], completion: GKChallengeComposeHandler?) -> UIViewController

Provides a view controller that you present to the player to issue an achievement challenge.

func challengeComposeController(withMessage: String?, players: [GKPlayer], completionHandler: GKChallengeComposeCompletionBlock?) -> UIViewController

Provides a view controller that you present to the player to issue an achievement challenge.

Deprecated

func challengeComposeController(withPlayers: [String]?, message: String?, completionHandler: GKChallengeComposeCompletionBlock?) -> UIViewController?

Provides a challenge compose view controller with preselected player identifiers and a message.

Deprecated

