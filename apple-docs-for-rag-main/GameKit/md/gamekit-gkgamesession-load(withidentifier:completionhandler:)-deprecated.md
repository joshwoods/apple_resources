

- GameKit
- GKGameSession
-  load(withIdentifier:completionHandler:) Deprecated

Type Method

# load(withIdentifier:completionHandler:)

Loads a specific game session.

iOS 10.0–12.0DeprecatediPadOS 10.0–12.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.12–10.14DeprecatedtvOS 10.0–12.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
class func load(
    withIdentifier identifier: String,
    completionHandler: @escaping (GKGameSession?, (any Error)?) -> Void
)
```

``` source
class func load(withIdentifier identifier: String) async throws -> GKGameSession
```

Deprecated

For real-time matches, use GKMatchmakerViewController. For turn-based matches, use GKTurnBasedMatchmakerViewController.

## Parameters 

`identifier`  

A unique string that identifies the game session to be loaded.

`completionHandler`  

A block that is called after the game session has been loaded.

session  
The `GKGameSession` object associated with the specified identifier.

error  
If an error occurred, this parameter holds an error object that explains the error. Otherwise, the value of this parameter is nil. See `GameKit Constants` for a list of error codes specific to GameKit.

## See Also

### Creating and Loading Game Sessions

class func createSession(inContainer: String?, withTitle: String, maxConnectedPlayers: Int, completionHandler: (GKGameSession?, (any Error)?) -> Void)

Creates a new game session inside of an iCloud container.

Deprecated

class func loadSessions(inContainer: String?, completionHandler: ([GKGameSession]?, (any Error)?) -> Void)

Retrieves all of the game sessions associated with a container.

Deprecated

class func remove(withIdentifier: String, completionHandler: ((any Error)?) -> Void)

Removes the specified game session.

Deprecated

