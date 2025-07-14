

- GameKit
- GKLocalPlayer
-  loadDefaultLeaderboardCategoryID(completionHandler:) Deprecated

Instance Method

# loadDefaultLeaderboardCategoryID(completionHandler:)

Loads the category identifier for the local player’s default leaderboard.

macOS 10.8–10.10DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

**macOS, visionOS, watchOS**

``` source
func loadDefaultLeaderboardCategoryID(completionHandler: ((String?, (any Error)?) -> Void)? = nil)
```

**visionOS**

``` source
func loadDefaultLeaderboardCategoryID() async throws -> String
```

Deprecated

Use loadDefaultLeaderboardIdentifier(completionHandler:) instead.

## Parameters 

`completionHandler`  

A block to call when the request completes.

The block receives the following parameters:

categoryID  
The category ID string for the local player’s default leaderboard.

error  
If an error occurrs, this parameter holds an error object that explains the error. Otherwise, the value of this parameter is `nil`.

## See Also

### Deprecated methods

func authenticate(completionHandler: (((any Error)?) -> Void)?)

Authenticates the local player on the device.

Deprecated

func generateIdentityVerificationSignature(completionHandler: ((URL?, Data?, Data?, UInt64, (any Error)?) -> Void)?)

Generates a signature so that a third-party server can authenticate the local player.

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

