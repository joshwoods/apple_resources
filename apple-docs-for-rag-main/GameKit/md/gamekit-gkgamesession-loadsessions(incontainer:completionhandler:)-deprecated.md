

- GameKit
- GKGameSession
-  loadSessions(inContainer:completionHandler:) Deprecated

Type Method

# loadSessions(inContainer:completionHandler:)

Retrieves all of the game sessions associated with a container.

iOS 10.0–12.0DeprecatediPadOS 10.0–12.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.12–10.14DeprecatedtvOS 10.0–12.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
class func loadSessions(
    inContainer containerName: String?,
    completionHandler: @escaping ([GKGameSession]?, (any Error)?) -> Void
)
```

``` source
class func loadSessions(inContainer containerName: String?) async throws -> [GKGameSession]
```

Deprecated

For real-time matches, use GKMatchmakerViewController. For turn-based matches, use GKTurnBasedMatchmakerViewController.

## Parameters 

`containerName`  

A unique string that identifies the container to be accessed.

`completionHandler`  

A block that is called after all the game sessions have been loaded.

sessions  
An array of `GKGameSession` objects that contains all of the game sessions associated with the specified container.

error  
If an error occurred, this parameter holds an error object that explains the error. Otherwise, the value of this parameter is nil. See `GameKit Constants` for a list of error codes specific to GameKit.

## See Also

### Creating and Loading Game Sessions

class func createSession(inContainer: String?, withTitle: String, maxConnectedPlayers: Int, completionHandler: (GKGameSession?, (any Error)?) -> Void)

Creates a new game session inside of an iCloud container.

Deprecated

class func load(withIdentifier: String, completionHandler: (GKGameSession?, (any Error)?) -> Void)

Loads a specific game session.

Deprecated

class func remove(withIdentifier: String, completionHandler: ((any Error)?) -> Void)

Removes the specified game session.

Deprecated

