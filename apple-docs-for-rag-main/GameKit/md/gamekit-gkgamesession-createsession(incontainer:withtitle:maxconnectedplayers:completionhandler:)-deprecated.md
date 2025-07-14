

- GameKit
- GKGameSession
-  createSession(inContainer:withTitle:maxConnectedPlayers:completionHandler:) Deprecated

Type Method

# createSession(inContainer:withTitle:maxConnectedPlayers:completionHandler:)

Creates a new game session inside of an iCloud container.

iOS 10.0–12.0DeprecatediPadOS 10.0–12.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.12–10.14DeprecatedtvOS 10.0–12.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
class func createSession(
    inContainer containerName: String?,
    withTitle title: String,
    maxConnectedPlayers maxPlayers: Int,
    completionHandler: @escaping (GKGameSession?, (any Error)?) -> Void
)
```

``` source
class func createSession(
    inContainer containerName: String?,
    withTitle title: String,
    maxConnectedPlayers maxPlayers: Int
) async throws -> GKGameSession
```

Deprecated

For real-time matches, use GKMatchmakerViewController. For turn-based matches, use GKTurnBasedMatchmakerViewController.

## Parameters 

`containerName`  

A `String` value representing the iCloud container for the game session.

`title`  

A `String` value representing the title of the game session.

`maxPlayers`  

An `Integer` value indicating the maximum number of players allowed in the game session.

`completionHandler`  

A block that is called after a new game session has been created.

gameSession  
A `GKGameSession` object containing information about the newly created game session.

error  
If an error occurred, this parameter holds an error object that explains the error. Otherwise, the value of this parameter is nil. See `GameKit Constants` for a list of error codes specific to GameKit.

## Discussion

The container name must be a valid iCloud container associated with your app. After a user has finished a game and is done with a game session, remove the created game session from iCloud using remove(withIdentifier:completionHandler:). See iCloud Design Guide for more information on incorporating iCloud in your app.

## See Also

### Creating and Loading Game Sessions

class func load(withIdentifier: String, completionHandler: (GKGameSession?, (any Error)?) -> Void)

Loads a specific game session.

Deprecated

class func loadSessions(inContainer: String?, completionHandler: ([GKGameSession]?, (any Error)?) -> Void)

Retrieves all of the game sessions associated with a container.

Deprecated

class func remove(withIdentifier: String, completionHandler: ((any Error)?) -> Void)

Removes the specified game session.

Deprecated

