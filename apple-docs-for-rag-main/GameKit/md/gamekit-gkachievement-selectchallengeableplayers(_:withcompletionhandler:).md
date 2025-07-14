

- GameKit
- GKAchievement
-  selectChallengeablePlayers(\_:withCompletionHandler:) 

Instance Method

# selectChallengeablePlayers(\_:withCompletionHandler:)

Finds the subset of players who can earn an achievement.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
func selectChallengeablePlayers(
    _ players: [GKPlayer],
    withCompletionHandler completionHandler: (([GKPlayer]?, (any Error)?) -> Void)? = nil
)
```

``` source
func selectChallengeablePlayers(_ players: [GKPlayer]) async throws -> [GKPlayer]
```

## Parameters 

`players`  

A list of players that GameKit uses to find players who are eligible to earn the achievement.

`completionHandler`  

A block that GameKit calls when this method completes.

The block receives the following parameters:

`challengeablePlayers`  
The players in the `players` parameter who are able to earn the achievement.

`error`  
Describes an error if it occurs, or `nil` if the operation completes.

## See Also

### Issuing Achievement Challenges

func challengeComposeController(withMessage: String?, players: [GKPlayer], completion: GKChallengeComposeHandler?) -> UIViewController

Provides a view controller that you present to the player to issue an achievement challenge.

typealias GKChallengeComposeHandler

A completion block that provides information about the player who issues a challenge and the players who receive it.

func challengeComposeController(withMessage: String?, players: [GKPlayer], completionHandler: GKChallengeComposeCompletionBlock?) -> UIViewController

Provides a view controller that you present to the player to issue an achievement challenge.

Deprecated

func challengeComposeController(withPlayers: [String]?, message: String?, completionHandler: GKChallengeComposeCompletionBlock?) -> UIViewController?

Provides a challenge compose view controller with preselected player identifiers and a message.

Deprecated

