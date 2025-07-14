

- WebKit
- WKPreferences
- WKPreferences.InactiveSchedulingPolicy
-  WKPreferences.InactiveSchedulingPolicy.none 

Case

# WKPreferences.InactiveSchedulingPolicy.none

A policy where a web view that’s not in a window runs tasks normally.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
case none
```

## See Also

### Scheduling policies

case suspend

A policy where a web view that’s not in a window fully suspends tasks.

case throttle

A policy where a web view that’s not in a window limits processing, but does not fully suspend tasks.

