

- GameKit
- GKSessionDelegate
-  session(\_:didFailWithError:) Deprecated

Instance Method

# session(\_:didFailWithError:)

Sent to the delegate when a serious error has occurred in the session.

macOS 10.8–10.10DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
optional func session(
    _ session: GKSession,
    didFailWithError error: any Error
)
```

## Parameters 

`session`  

The session that failed.

`error`  

The error that occurred.

## Discussion

This method is called when a serious internal error occurred in the session. Your application should disconnect the session from other peers and release the session.

## See Also

### Connection Errors

func session(GKSession, connectionWithPeerFailed: String, withError: any Error)

Received by the delegate when an attempt to connect to another peer failed.

Deprecated

