

- WatchKit
- WKExtendedRuntimeSession
-  requestAutoLaunchAuthorizationStatus(completion:) 

Type Method

# requestAutoLaunchAuthorizationStatus(completion:)

watchOS 9.0+

``` source
class func requestAutoLaunchAuthorizationStatus(completion: @escaping (WKExtendedRuntimeSessionAutoLaunchAuthorizationStatus, (any Error)?) -> Void)
```

``` source
class func requestAutoLaunchAuthorizationStatus() async throws -> WKExtendedRuntimeSessionAutoLaunchAuthorizationStatus
```

## See Also

### Managing the Session State

func start()

Starts running the session.

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

enum WKExtendedRuntimeSessionAutoLaunchAuthorizationStatus

