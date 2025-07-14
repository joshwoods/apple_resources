

- WatchKit
-  WKExtendedRuntimeSessionState 

Enumeration

# WKExtendedRuntimeSessionState

The activation states for an extended runtime session.

watchOS 6.0+

``` source
enum WKExtendedRuntimeSessionState
```

## Topics

### Session States

case notStarted

The app has not yet started or scheduled the session.

case scheduled

The app has scheduled the session to run at a future date.

case running

The session is actively running.

case invalid

Either the session has encountered an error, or it has stopped running.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

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

var expirationDate: Date?

The time and date when the session expires.

class func requestAutoLaunchAuthorizationStatus(completion: (WKExtendedRuntimeSessionAutoLaunchAuthorizationStatus, (any Error)?) -> Void)

enum WKExtendedRuntimeSessionAutoLaunchAuthorizationStatus

