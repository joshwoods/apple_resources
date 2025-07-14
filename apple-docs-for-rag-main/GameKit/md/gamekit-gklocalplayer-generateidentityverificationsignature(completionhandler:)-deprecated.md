

- GameKit
- GKLocalPlayer
-  generateIdentityVerificationSignature(completionHandler:) Deprecated

Instance Method

# generateIdentityVerificationSignature(completionHandler:)

Generates a signature so that a third-party server can authenticate the local player.

iOS 7.0–13.5DeprecatediPadOS 7.0–13.5DeprecatedMac Catalyst 13.1–13.5DeprecatedmacOS 10.10–10.15.5DeprecatedtvOS 9.0–13.4.8DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–6.5Deprecated

``` source
func generateIdentityVerificationSignature(completionHandler: ((URL?, Data?, Data?, UInt64, (any Error)?) -> Void)? = nil)
```

``` source
func generateIdentityVerificationSignature() async throws -> (URL, Data, Data, UInt64)
```

Deprecated

Use fetchItems(forIdentityVerificationSignature:) instead.

## Parameters 

`completionHandler`  

A block to call when the request completes.

The block receives the following parameters:

publicKeyUrl  
The URL for the public encryption key.

signature  
The verification signature data that GameKit generates.

salt  
A random `NSString` that GameKit uses to compute the hash and randomize it.

timestamp  
The signature’s creation date and time.

error  
If an error occurrs, this parameter holds an error object that explains the error. Otherwise, the value of this parameter is `nil`.

## Discussion

To generate a signature on your server, see the fetchItems(forIdentityVerificationSignature:) method.

## See Also

### Deprecated methods

func authenticate(completionHandler: (((any Error)?) -> Void)?)

Authenticates the local player on the device.

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

