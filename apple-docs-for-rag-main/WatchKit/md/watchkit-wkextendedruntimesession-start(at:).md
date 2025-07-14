

- WatchKit
- WKExtendedRuntimeSession
-  start(at:) 

Instance Method

# start(at:)

Schedules a session to start running at a future date.

watchOS 6.0+

``` source
func start(at date: Date)
```

## Parameters 

`date`  

The time and date when the session starts running.

## Mentioned in 

Using extended runtime sessions

## Discussion

Use start(at:) to set up a scheduable session. You must call this method while your app is running in the foreground. However, when the scheduled date and time arrives, the session starts running regardless of your app’s current state. If your app isn’t running, the system launches your app and calls your extension delegate’s handle(_:) method to start the session. If you don’t set the session’s delegate in the handle(_:) method, the system ends the session.

Important

You can only use this method for alarm sessions.

If you call this method with a date that has already passed, the system tries to immediately starts the session, but the session is only given 30 minutes from the provided date. If the date is more than one minute in the past, this method fails.

## See Also

### Managing the Session State

func start()

Starts running the session.

func invalidate()

Stops the session.

var state: WKExtendedRuntimeSessionState

The session’s current state.

enum WKExtendedRuntimeSessionState

The activation states for an extended runtime session.

var expirationDate: Date?

The time and date when the session expires.

class func requestAutoLaunchAuthorizationStatus(completion: (WKExtendedRuntimeSessionAutoLaunchAuthorizationStatus, (any Error)?) -> Void)

enum WKExtendedRuntimeSessionAutoLaunchAuthorizationStatus

