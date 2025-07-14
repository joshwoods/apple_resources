

- WatchKit
- WKExtendedRuntimeSessionDelegate
-  extendedRuntimeSessionDidStart(\_:) 

Instance Method

# extendedRuntimeSessionDidStart(\_:)

Indicates that the session has started running.

watchOS 6.0+

``` source
func extendedRuntimeSessionDidStart(_ extendedRuntimeSession: WKExtendedRuntimeSession)
```

**Required**

## Parameters 

`extendedRuntimeSession`  

The session that started running.

## Discussion

The system calls this method when your session starts running, in response to the start() method, or because a scheduled session’s start date has arrived.

## See Also

### Monitoring State Changes

func extendedRuntimeSessionWillExpire(WKExtendedRuntimeSession)

Indicates that the session is about to expire.

**Required**

func extendedRuntimeSession(WKExtendedRuntimeSession, didInvalidateWith: WKExtendedRuntimeSessionInvalidationReason, error: (any Error)?)

Indicates that the session has encountered an error or stopped running.

**Required**

enum WKExtendedRuntimeSessionInvalidationReason

The reasons why a session can become invalid.

