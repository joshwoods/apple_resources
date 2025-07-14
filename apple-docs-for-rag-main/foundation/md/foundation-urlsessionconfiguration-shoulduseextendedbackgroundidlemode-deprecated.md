

- Foundation
- URLSessionConfiguration
-  shouldUseExtendedBackgroundIdleMode Deprecated

Instance Property

# shouldUseExtendedBackgroundIdleMode

A Boolean value that indicates whether TCP connections should be kept open when the app moves to the background.

iOS 9.0–18.4DeprecatediPadOS 9.0–18.4DeprecatedMac Catalyst 13.1–18.4DeprecatedmacOS 10.11–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 2.0–11.4Deprecated

``` source
var shouldUseExtendedBackgroundIdleMode: Bool { get set }
```

Deprecated

Not supported

## Discussion

In addition to requesting that the connection be kept open, setting this value to true asks the system to delay reclaiming the connection when the app moves to the background.

## See Also

### Related Documentation

Networking and Multitasking

### Supporting background transfers

var sessionSendsLaunchEvents: Bool

A Boolean value that indicates whether the app should be resumed or launched in the background when transfers finish.

var isDiscretionary: Bool

A Boolean value that determines whether background tasks can be scheduled at the discretion of the system for optimal performance.

