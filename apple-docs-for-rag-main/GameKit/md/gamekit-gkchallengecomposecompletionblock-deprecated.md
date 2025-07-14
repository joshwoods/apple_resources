

- GameKit
-  GKChallengeComposeCompletionBlock Deprecated

Type Alias

# GKChallengeComposeCompletionBlock

A completion block that provides information about the player who issues a challenge and the players who receive it.

iOS 8.0–17.0DeprecatediPadOS 8.0–17.0DeprecatedMac Catalyst 13.1–17.0DeprecatedmacOS 10.10–14.0DeprecatedtvOS 9.0–17.0DeprecatedvisionOS 1.0–1.0Deprecated

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
typealias GKChallengeComposeCompletionBlock = (UIViewController, Bool, [String]?) -> Void
```

**macOS**

``` source
typealias GKChallengeComposeCompletionBlock = (NSViewController, Bool, [String]?) -> Void
```

## Parameters 

`composeController`  

View controller for the challenge.

`didIssueChallenge`  

A Boolean value that indicates whether the player issues the challenge.

`sentPlayerIDs`  

The identifiers for the players that receive the challenge.

## See Also

### Deprecated symbols

var issuingPlayerID: String?

The player who issues the challenge.

Deprecated

var receivingPlayerID: String?

The player who receives the challenge.

Deprecated

