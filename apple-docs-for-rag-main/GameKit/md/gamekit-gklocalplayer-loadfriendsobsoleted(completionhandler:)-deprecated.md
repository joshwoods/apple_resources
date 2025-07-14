

- GameKit
- GKLocalPlayer
-  loadFriendsObsoleted(completionHandler:) Deprecated

Instance Method

# loadFriendsObsoleted(completionHandler:)

Retrieves a list of player identifiers for the local player’s friends.

iOS 4.1–8.0DeprecatediPadOS 4.1–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.8–10.10DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

**iOS, iPadOS, Mac Catalyst, macOS, visionOS, watchOS**

``` source
func loadFriendsObsoleted(completionHandler: (([String]?, (any Error)?) -> Void)? = nil)
```

**Mac Catalyst, visionOS**

``` source
func loadFriendsObsoleted() async throws -> [String]
```

Deprecated

Use loadFriends(_:) instead.

## Parameters 

`completionHandler`  

A block to call when the request completes.

The block receives the following parameters:

friendIDs  
An array of `NSString` objects containing the player identifiers for the players who are friends of the local player. If an error occurs, this value can be non-`nil`. In that case, the array contains the data that GameKit downloads before the error occurs.

error  
If an error occurs, this parameter holds an error object that explains the error. Otherwise, the value of this parameter is `nil`.

## Discussion

After this call completes, the friends property of the shared local player object is the same list of players that the completion handler returns.

## See Also

### Related Documentation

var friends: [String]?

The player identifiers for the local player’s friends.

Deprecated

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

func setDefaultLeaderboardCategoryID(String?, completionHandler: (((any Error)?) -> Void)?)

Sets the category identifier for the local player’s default leaderboard.

Deprecated

