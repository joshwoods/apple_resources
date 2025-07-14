

- WebKit
- WKPreferences
- WKPreferences.InactiveSchedulingPolicy
-  WKPreferences.InactiveSchedulingPolicy.suspend 

Case

# WKPreferences.InactiveSchedulingPolicy.suspend

A policy where a web view that’s not in a window fully suspends tasks.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
case suspend
```

## See Also

### Scheduling policies

case none

A policy where a web view that’s not in a window runs tasks normally.

case throttle

A policy where a web view that’s not in a window limits processing, but does not fully suspend tasks.

