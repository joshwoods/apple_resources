

- GameKit
- GKLocalPlayer
-  setDefaultLeaderboardCategoryID(\_:completionHandler:) Deprecated

Instance Method

# setDefaultLeaderboardCategoryID(\_:completionHandler:)

Sets the category identifier for the local player’s default leaderboard.

macOS 10.8–10.10DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

**macOS, visionOS, watchOS**

``` source
func setDefaultLeaderboardCategoryID(
    _ categoryID: String?,
    completionHandler: (((any Error)?) -> Void)? = nil
)
```

**visionOS**

``` source
func setDefaultLeaderboardCategoryID(_ categoryID: String?) async throws
```

Deprecated

Use setDefaultLeaderboardIdentifier(_:completionHandler:) instead.

## Parameters 

`categoryID`  

The category ID string for one of your game’s leaderboards.

`completionHandler`  

A block to call when the request completes.

The block receives the following parameter:

error  
If an error occurs, this parameter holds an error object that explains the error. Otherwise, the value of this parameter is `nil`.

## Discussion

You set the default leaderboard in App Store Connect when you configure your game’s leaderboards. All players normally start with this leaderboard as the default leaderboard. Calling this method changes the default leaderboard only for the local player.

## See Also

### Deprecated methods

func authenticate(completionHandler: (((any Error)?) -> Void)?)

Authenticates the local player on the device.

Deprecated

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

