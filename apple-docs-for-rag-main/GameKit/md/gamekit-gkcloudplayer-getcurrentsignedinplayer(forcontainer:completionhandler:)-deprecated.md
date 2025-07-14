

- GameKit
- GKCloudPlayer
-  getCurrentSignedInPlayer(forContainer:completionHandler:) Deprecated

Type Method

# getCurrentSignedInPlayer(forContainer:completionHandler:)

Returns player information for the currently signed-in player.

iOS 10.0–12.0DeprecatediPadOS 10.0–12.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.12–10.14DeprecatedtvOS 10.0–12.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
class func getCurrentSignedInPlayer(
    forContainer containerName: String?,
    completionHandler handler: @escaping (GKCloudPlayer?, (any Error)?) -> Void
)
```

``` source
class func currentSignedInPlayer(forContainer containerName: String?) async throws -> GKCloudPlayer
```

## Parameters 

`containerName`  

String containing a unique container name associated with the app.

`handler`  

A block that is called after the player information is retrieved.

player  
The GKCloudPlayer object representing the currently signed-in player.

error  
If an error occurred, this parameter holds an error object that explains the error. Otherwise, the value of this parameter is `nil`. See `GameKit Constants`for a list of error codes specific to GameKit.

## Discussion

The container name must be a unique string associated with the app.

