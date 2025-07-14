

- WatchKit
- WKExtendedRuntimeSession
-  state 

Instance Property

# state

The session’s current state.

watchOS 6.0+

``` source
var state: WKExtendedRuntimeSessionState { get }
```

## Discussion

For a list of session states, see WKExtendedRuntimeSessionState.

## See Also

### Managing the Session State

func start()

Starts running the session.

func start(at: Date)

Schedules a session to start running at a future date.

func invalidate()

Stops the session.

enum WKExtendedRuntimeSessionState

The activation states for an extended runtime session.

var expirationDate: Date?

The time and date when the session expires.

class func requestAutoLaunchAuthorizationStatus(completion: (WKExtendedRuntimeSessionAutoLaunchAuthorizationStatus, (any Error)?) -> Void)

enum WKExtendedRuntimeSessionAutoLaunchAuthorizationStatus

