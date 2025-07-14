

- WatchKit
- WKExtendedRuntimeSessionDelegate
-  extendedRuntimeSession(\_:didInvalidateWith:error:) 

Instance Method

# extendedRuntimeSession(\_:didInvalidateWith:error:)

Indicates that the session has encountered an error or stopped running.

watchOS 6.0+

``` source
func extendedRuntimeSession(
    _ extendedRuntimeSession: WKExtendedRuntimeSession,
    didInvalidateWith reason: WKExtendedRuntimeSessionInvalidationReason,
    error: (any Error)?
)
```

**Required**

## Parameters 

`extendedRuntimeSession`  

The session that became invalid.

`reason`  

The reason the session became invalid.

`error`  

If the `reason` parameter is WKExtendedRuntimeSessionInvalidationReason.error, then this parameter contains additional information about the error. Otherwise it is set to `nil`.

## Discussion

The system calls this method both when a session fails to start and when a session stops running. Use the invalidation reason to determine why the session became invalid.

Important

If your app terminates immediately after the system invalidates the session, you may not receive this delegate call until the user launches your app again. In that case, the system calls your extension delegate’s handle(_:) method to resume the session. Then, after you assign the session delegate, the system finally makes this delegate call.

## See Also

### Monitoring State Changes

func extendedRuntimeSessionDidStart(WKExtendedRuntimeSession)

Indicates that the session has started running.

**Required**

func extendedRuntimeSessionWillExpire(WKExtendedRuntimeSession)

Indicates that the session is about to expire.

**Required**

enum WKExtendedRuntimeSessionInvalidationReason

The reasons why a session can become invalid.

