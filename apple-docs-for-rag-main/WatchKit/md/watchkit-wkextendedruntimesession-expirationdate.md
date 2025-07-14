

- WatchKit
- WKExtendedRuntimeSession
-  expirationDate 

Instance Property

# expirationDate

The time and date when the session expires.

watchOS 6.0+

``` source
var expirationDate: Date? { get }
```

## Mentioned in 

Using extended runtime sessions

## Discussion

Use this property to determine how much time remains before the session stops running.

This property starts set to `nil`. The system assigns a date as soon as the session starts running. This property remains valid, even after the session becomes invalid.

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

class func requestAutoLaunchAuthorizationStatus(completion: (WKExtendedRuntimeSessionAutoLaunchAuthorizationStatus, (any Error)?) -> Void)

enum WKExtendedRuntimeSessionAutoLaunchAuthorizationStatus

