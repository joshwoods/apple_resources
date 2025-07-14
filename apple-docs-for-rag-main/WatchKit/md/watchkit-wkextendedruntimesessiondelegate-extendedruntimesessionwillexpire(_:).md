

- WatchKit
- WKExtendedRuntimeSessionDelegate
-  extendedRuntimeSessionWillExpire(\_:) 

Instance Method

# extendedRuntimeSessionWillExpire(\_:)

Indicates that the session is about to expire.

watchOS 6.0+

``` source
func extendedRuntimeSessionWillExpire(_ extendedRuntimeSession: WKExtendedRuntimeSession)
```

**Required**

## Parameters 

`extendedRuntimeSession`  

The session that is about to expire.

## Discussion

The system only grants each session a limited amount of time to run. The system calls this method just before reaching that limit. Implement this method to finish any tasks and clean up before the session ends.

## See Also

### Monitoring State Changes

func extendedRuntimeSessionDidStart(WKExtendedRuntimeSession)

Indicates that the session has started running.

**Required**

func extendedRuntimeSession(WKExtendedRuntimeSession, didInvalidateWith: WKExtendedRuntimeSessionInvalidationReason, error: (any Error)?)

Indicates that the session has encountered an error or stopped running.

**Required**

enum WKExtendedRuntimeSessionInvalidationReason

The reasons why a session can become invalid.

