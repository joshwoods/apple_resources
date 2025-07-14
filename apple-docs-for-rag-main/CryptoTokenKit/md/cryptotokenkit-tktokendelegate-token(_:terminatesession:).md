

- CryptoTokenKit
- TKTokenDelegate
-  token(\_:terminateSession:) 

Instance Method

# token(\_:terminateSession:)

Tells the delegate to terminate the specified token session.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
optional func token(
    _ token: TKToken,
    terminateSession session: TKTokenSession
)
```

## Parameters 

`token`  

The token.

`session`  

The token session to be terminated.

## See Also

### Delegate Methods

func createSession(TKToken) throws -> TKTokenSession

Tells the delegate to create a session for the specified token.

**Required**

