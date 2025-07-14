

- WatchKit
-  WKExtendedRuntimeSessionAutoLaunchAuthorizationStatus 

Enumeration

# WKExtendedRuntimeSessionAutoLaunchAuthorizationStatus

watchOS 9.0+

``` source
enum WKExtendedRuntimeSessionAutoLaunchAuthorizationStatus
```

## Topics

### Enumeration Cases

case active

case inactive

case unknown

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

enum WKExtendedRuntimeSessionState

The activation states for an extended runtime session.

var expirationDate: Date?

The time and date when the session expires.

class func requestAutoLaunchAuthorizationStatus(completion: (WKExtendedRuntimeSessionAutoLaunchAuthorizationStatus, (any Error)?) -> Void)

