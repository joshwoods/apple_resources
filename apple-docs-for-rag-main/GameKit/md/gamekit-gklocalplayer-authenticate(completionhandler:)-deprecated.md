

- GameKit
- GKLocalPlayer
-  authenticate(completionHandler:) Deprecated

Instance Method

# authenticate(completionHandler:)

Authenticates the local player on the device.

visionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

**visionOS, watchOS**

``` source
func authenticate(completionHandler: (((any Error)?) -> Void)? = nil)
```

**visionOS**

``` source
func authenticate() async throws
```

Deprecated

Use authenticateHandler instead.

## Parameters 

`completionHandler`  

A block to call when the player authenticates or when an error occurs.

The block takes the following parameter:

error  
This parameter is `nil` if the player successfully authenticates. Otherwise, it contains an error object that describes the error that occurrs.

## Discussion

For more information, see Authenticating a player.

## See Also

### Deprecated methods

func generateIdentityVerificationSignature(completionHandler: ((URL?, Data?, Data?, UInt64, (any Error)?) -> Void)?)

Generates a signature so that a third-party server can authenticate the local player.

Deprecated

func loadDefaultLeaderboardCategoryID(completionHandler: ((String?, (any Error)?) -> Void)?)

Loads the category identifier for the local player’s default leaderboard.

Deprecated

func loadFriendPlayers(completionHandler: (([GKPlayer]?, (any Error)?) -> Void)?)

Retrieves a list of player identifiers for the local player’s friends.

Deprecated

func loadFriendsObsoleted(completionHandler: (([String]?, (any Error)?) -> Void)?)

Retrieves a list of player identifiers for the local player’s friends.

Deprecated

func setDefaultLeaderboardCategoryID(String?, completionHandler: (((any Error)?) -> Void)?)

Sets the category identifier for the local player’s default leaderboard.

Deprecated

