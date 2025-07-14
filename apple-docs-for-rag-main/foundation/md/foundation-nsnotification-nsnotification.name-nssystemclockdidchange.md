

- Foundation
- NSNotification
- NSNotification.Name
-  NSSystemClockDidChange 

Type Property

# NSSystemClockDidChange

A notification posted whenever the system clock is changed.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let NSSystemClockDidChange: NSNotification.Name
```

## Discussion

This can be initiated by a call to `settimeofday(_:_:)` or the user changing values in the Date and Time Preference panel.

The notification object is `null`. This notification does not contain a `userInfo` dictionary.

