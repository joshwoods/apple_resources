

- Nearby Interaction
- NISessionDelegate
-  session(\_:didInvalidateWith:) 

Instance Method

# session(\_:didInvalidateWith:)

Notifies you of an invalidated session.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+watchOS 7.3+

``` source
optional func session(
    _ session: NISession,
    didInvalidateWith error: any Error
)
```

## Parameters 

`session`  

The invalidated session.

`error`  

The error that invalidated the session.

## Mentioned in 

Initiating and maintaining a session

## Discussion

The delegate of an invalidated session receives no further callbacks, and the app can’t restart the session. To resume peer interaction, remove references to the invalidated session and begin a new session.

