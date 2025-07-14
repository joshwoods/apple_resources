

- GameKit
- GKLocalPlayer
-  loadFriendPlayers(completionHandler:) Deprecated

Instance Method

# loadFriendPlayers(completionHandler:)

Retrieves a list of player identifiers for the local player’s friends.

iOS 8.0–10.0DeprecatediPadOS 8.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.10–10.11DeprecatedtvOS 9.0–10.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS, watchOS**

``` source
func loadFriendPlayers(completionHandler: (([GKPlayer]?, (any Error)?) -> Void)? = nil)
```

**Mac Catalyst, visionOS**

``` source
func loadFriendPlayers() async throws -> [GKPlayer]
```

Deprecated

Use loadFriends(_:) instead.

## Parameters 

`completionHandler`  

A block to call when the request completes.

The block receives the following parameters:

friendPlayers  
An array of GKPlayer objects containing the player identifiers for the players who are friends of the local player. If an error occurs, this value can be non-`nil`. In that case, the array contains the data that GameKit downloads before the error occurs.

error  
If an error occurs, this parameter holds an error object that explains the error. Otherwise, the value of this parameter is `nil`.

## Discussion

The code below shows an example of how to load a player’s friends. Create your own method to save information about the found players.

```
- (void) retrieveFriends
{
   GKLocalPlayer *lp = [GKLocalPlayer localPlayer];
   if (lp.authenticated)
   {
      [lp loadFriendPlayersWithCompletionHandler:^(NSArray *friendPlayers, NSError *error) {
         if (friendPlayers != nil)
         {
            [self loadPlayerData: friendPlayers];
         }
      }];
   }
}
```

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

func loadFriendsObsoleted(completionHandler: (([String]?, (any Error)?) -> Void)?)

Retrieves a list of player identifiers for the local player’s friends.

Deprecated

func setDefaultLeaderboardCategoryID(String?, completionHandler: (((any Error)?) -> Void)?)

Sets the category identifier for the local player’s default leaderboard.

Deprecated

