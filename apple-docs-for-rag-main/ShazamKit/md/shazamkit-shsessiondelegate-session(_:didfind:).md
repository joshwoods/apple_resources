

- ShazamKit
- SHSessionDelegate
-  session(\_:didFind:) 

Instance Method

# session(\_:didFind:)

Tells the delegate that the query signature matches an item in the catalog.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
optional func session(
    _ session: SHSession,
    didFind match: SHMatch
)
```

## Parameters 

`session`  

The session object that performs the match.

`match`  

The matching items from the catalog.

## See Also

### Handling matches

func session(SHSession, didNotFindMatchFor: SHSignature, error: (any Error)?)

Tells the delegate that the query signature doesn’t match an item in the catalog, or that there’s an error.

