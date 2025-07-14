

- GameKit
- GKMatchmaker
-  match(for:completionHandler:) 

Instance Method

# match(for:completionHandler:)

Creates a match from an invitation that the local player accepts.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
func match(
    for invite: GKInvite,
    completionHandler: ((GKMatch?, (any Error)?) -> Void)? = nil
)
```

``` source
func match(for invite: GKInvite) async throws -> GKMatch
```

## Parameters 

`invite`  

The invitation that the local player accepts.

`completionHandler`  

The block that GameKit calls when it completes the request.

This block receives the following parameters:

`match`  
The match that GameKit creates when the local player accepts the invitation. If unsuccessful, this parameter is `nil`.

`error`  
Describes an error if one occurs, or `nil` if the operation completes.

## Discussion

Use this method when you implement your own interface to inform you when the local player joins a match.

