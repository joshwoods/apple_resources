

- CarKey
- CarKeyRemoteControlSessionDelegate
-  remoteControlSession(\_:didInvalidateWithError:) 

Instance Method

# remoteControlSession(\_:didInvalidateWithError:)

Notifies your delegate object that the session become invalid for the specified reason.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.3+watchOS 9.0+

``` source
func remoteControlSession(
    _ session: CarKeyRemoteControlSession,
    didInvalidateWithError: CarKeyErrorCode
)
```

**Required**

## Parameters 

`session`  

The session that became invalid.

`didInvalidateWithError`  

The error code that contains the reason for the invalid session. For a list of possible values, see CarKeyErrorCode.

## Discussion

Use this method to detect if the system invalidated the session for any reason. The system executes this method on the dispatch queue you specified when you started the session.

