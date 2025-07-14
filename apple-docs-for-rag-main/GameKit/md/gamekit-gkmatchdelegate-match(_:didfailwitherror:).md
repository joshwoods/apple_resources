

- GameKit
- GKMatchDelegate
-  match(\_:didFailWithError:) 

Instance Method

# match(\_:didFailWithError:)

Handles the local player’s connection errors to a match.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
optional func match(
    _ match: GKMatch,
    didFailWithError error: (any Error)?
)
```

## Parameters 

`match`  

The match in which the error occurs.

`error`  

The error that occurs.

## Discussion

GameKit calls this method when the local player can’t connect to any other players in the match.

