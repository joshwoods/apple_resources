

- WebKit
- WKPreferences
- WKPreferences.InactiveSchedulingPolicy
-  WKPreferences.InactiveSchedulingPolicy.throttle 

Case

# WKPreferences.InactiveSchedulingPolicy.throttle

A policy where a web view that’s not in a window limits processing, but does not fully suspend tasks.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
case throttle
```

## See Also

### Scheduling policies

case none

A policy where a web view that’s not in a window runs tasks normally.

case suspend

A policy where a web view that’s not in a window fully suspends tasks.

