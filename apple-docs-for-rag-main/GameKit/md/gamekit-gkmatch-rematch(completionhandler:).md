

- GameKit
- GKMatch
-  rematch(completionHandler:) 

Instance Method

# rematch(completionHandler:)

Creates a new match with the players from an existing match.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
func rematch(completionHandler: ((GKMatch?, (any Error)?) -> Void)? = nil)
```

``` source
func rematch() async throws -> GKMatch
```

## Parameters 

`completionHandler`  

The block that GameKit calls when it completes the request.

The block receives the following parameters:

`match`  
A new match, or `nil` if an error occurs.

`error`  
Describes an error if it occurs, or `nil` if the operation completes.

## Discussion

This method uses automatching to recreate a previous match. If you use this method to create a match, each instance of your game on each device should call this same method.

## See Also

### Finishing the match

func disconnect()

Disconnects the local player from the match.

