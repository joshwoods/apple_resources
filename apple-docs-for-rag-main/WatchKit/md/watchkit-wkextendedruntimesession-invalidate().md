

- WatchKit
- WKExtendedRuntimeSession
-  invalidate() 

Instance Method

# invalidate()

Stops the session.

watchOS 6.0+

``` source
func invalidate()
```

## Mentioned in 

Using extended runtime sessions

## Discussion

This method stops a running session. If you’ve scheduled a session, it cancels the session. If the session isn’t yet running or scheduled, this method triggers a WKExtendedRuntimeSessionErrorCode.notYetStarted error.

For sessions started with start(at:), you can only call invalidate() when the app is active. For all other sessions, you can call invalidate() to end a session at any time.

After calling invalidate(), you can no longer run the session. Create and start a new session instead.

## See Also

### Managing the Session State

func start()

Starts running the session.

func start(at: Date)

Schedules a session to start running at a future date.

var state: WKExtendedRuntimeSessionState

The session’s current state.

enum WKExtendedRuntimeSessionState

The activation states for an extended runtime session.

var expirationDate: Date?

The time and date when the session expires.

class func requestAutoLaunchAuthorizationStatus(completion: (WKExtendedRuntimeSessionAutoLaunchAuthorizationStatus, (any Error)?) -> Void)

enum WKExtendedRuntimeSessionAutoLaunchAuthorizationStatus

