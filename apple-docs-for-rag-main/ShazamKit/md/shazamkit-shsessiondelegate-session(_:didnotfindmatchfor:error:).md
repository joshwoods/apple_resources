

- ShazamKit
- SHSessionDelegate
-  session(\_:didNotFindMatchFor:error:) 

Instance Method

# session(\_:didNotFindMatchFor:error:)

Tells the delegate that the query signature doesn’t match an item in the catalog, or that there’s an error.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
optional func session(
    _ session: SHSession,
    didNotFindMatchFor signature: SHSignature,
    error: (any Error)?
)
```

## Parameters 

`session`  

The session object that performs the match.

`signature`  

The query signature to use for the match.

`error`  

The error that occurs; otherwise, `nil`, which indicates that there’s no match.

## Mentioned in 

Matching audio using the built-in microphone

## Discussion

You can retry the match if the error indicates an issue in communicating with the catalog server, such as SHError.Code.matchAttemptFailed.

## See Also

### Handling matches

func session(SHSession, didFind: SHMatch)

Tells the delegate that the query signature matches an item in the catalog.

