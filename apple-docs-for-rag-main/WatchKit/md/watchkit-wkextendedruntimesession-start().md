

- WatchKit
- WKExtendedRuntimeSession
-  start() 

Instance Method

# start()

Starts running the session.

watchOS 6.0+

``` source
func start()
```

## Mentioned in 

Using extended runtime sessions

## Discussion

Use start() to begin a session. You must call this method while your app is running in the foreground.

You can’t use the start() method to set up a schedulable session (such as a smart alarm session). Call the start(at:) method instead.

## See Also

### Managing the Session State

func start(at: Date)

Schedules a session to start running at a future date.

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

