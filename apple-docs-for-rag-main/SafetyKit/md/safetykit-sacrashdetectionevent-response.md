

- SafetyKit
- SACrashDetectionEvent
-  response 

Instance Property

# response

An indication of whether the system attempted to call an Emergency SOS provider.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+watchOS 10.1+

``` source
var response: SACrashDetectionEvent.Response { get }
```

## See Also

### Determining the event type

enum Response

An enumeration that defines possible emergency responses to a Crash Detection event.

var date: Date

The date and time the crash occurred.

var location: CLLocation?

The longitude and latitude where the crash detection occurred.

