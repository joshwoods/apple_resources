

- GameKit
- GKGameSession
-  remove(withIdentifier:completionHandler:) Deprecated

Type Method

# remove(withIdentifier:completionHandler:)

Removes the specified game session.

iOS 10.0–12.0DeprecatediPadOS 10.0–12.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.12–10.14DeprecatedtvOS 10.0–12.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
class func remove(
    withIdentifier identifier: String,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
class func remove(withIdentifier identifier: String) async throws
```

Deprecated

For real-time matches, use GKMatchmakerViewController. For turn-based matches, use GKTurnBasedMatchmakerViewController.

## Parameters 

`identifier`  

The unique string that identifies the game session to be removed.

`completionHandler`  

A block that is called after a game session has been removed from a container.

error  
If an error occurred, this parameter holds an error object that explains the error. Otherwise, the value of this parameter is nil. See `GameKit Constants` for a list of error codes specific to GameKit.

## Discussion

After the user has finished a game or decides to abandon a game, you must use this function to remove the game session from iCloud. Game sessions are not removed from iCloud automatically.

## See Also

### Creating and Loading Game Sessions

class func createSession(inContainer: String?, withTitle: String, maxConnectedPlayers: Int, completionHandler: (GKGameSession?, (any Error)?) -> Void)

Creates a new game session inside of an iCloud container.

Deprecated

class func load(withIdentifier: String, completionHandler: (GKGameSession?, (any Error)?) -> Void)

Loads a specific game session.

Deprecated

class func loadSessions(inContainer: String?, completionHandler: ([GKGameSession]?, (any Error)?) -> Void)

Retrieves all of the game sessions associated with a container.

Deprecated

