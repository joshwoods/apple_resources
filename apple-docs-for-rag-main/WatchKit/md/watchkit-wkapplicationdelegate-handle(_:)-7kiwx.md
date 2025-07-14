

- WatchKit
- WKApplicationDelegate
-  handle(\_:) 

Instance Method

# handle(\_:)

Tells the delegate that the system launched your app to resume an extended runtime session.

watchOS 7.0+

``` source
@MainActor
optional func handle(_ extendedRuntimeSession: WKExtendedRuntimeSession)
```

## Parameters 

`extendedRuntimeSession`  

The extended runtime session that the system is resuming.

## Discussion

The system calls this method after launching your app in response to a scheduled extended runtime session. This occurs if your app terminates after scheduling a session but before that session’s start date. The system may also call this method if your app crashes during an extended runtime session, letting you resume that session.

When implementing this method, set the session’s delegate to resume the session. If you don’t set the session’s delegate, the system ends the session.

