

- WatchKit
-  WKExtendedRuntimeSession 

Class

# WKExtendedRuntimeSession

A session that continues to run your app after the user has stopped interacting.

watchOS 6.0+

``` source
class WKExtendedRuntimeSession
```

## Mentioned in 

Using extended runtime sessions

Using background tasks

## Overview

With extended runtime sessions, your app continues to run after the user stops interacting with it. The app can continue to communicate with Bluetooth devices, process data, or play sounds or haptics, even after the watch’s screen turns off.

Each app can support a single type of extended runtime session: self care, mindfulness, physical therapy, or smart alarm. Select the session by enabling the appropriate Background Modes capability.

For more information, see Using extended runtime sessions.

## Topics

### Creating a Session

var delegate: (any WKExtendedRuntimeSessionDelegate)?

A delegate object for monitoring the session and responding to state changes and errors.

protocol WKExtendedRuntimeSessionDelegate

A set of optional methods for monitoring an extended runtime session.

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

enum WKExtendedRuntimeSessionAutoLaunchAuthorizationStatus

### Alerting the User

func notifyUser(hapticType: WKHapticType, repeatHandler: ((UnsafeMutablePointer&lt;WKHapticType>) -> TimeInterval)?)

Play a repeating haptic alert.

### Handling Errors

enum WKExtendedRuntimeSessionErrorCode

The error codes reported by extended runtime sessions.

let WKExtendedRuntimeSessionErrorDomain: String

The domain for errors reported by extended runtime sessions.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Runtime management

Background execution

Manage background sessions and tasks.

Life cycles

Receive and respond to life-cycle notifications.

Using extended runtime sessions

Create an extended runtime session that continues running your app after the user stops interacting with it.

Interacting with Bluetooth peripherals during background app refresh

Keep your complications up-to-date by reading values from a Bluetooth peripheral while your app is running in the background.

