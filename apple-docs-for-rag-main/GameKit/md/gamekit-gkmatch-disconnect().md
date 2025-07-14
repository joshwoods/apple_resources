

- GameKit
- GKMatch
-  disconnect() 

Instance Method

# disconnect()

Disconnects the local player from the match.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
func disconnect()
```

## Discussion

Call this method before ending a match.

## See Also

### Finishing the match

func rematch(completionHandler: ((GKMatch?, (any Error)?) -> Void)?)

Creates a new match with the players from an existing match.

