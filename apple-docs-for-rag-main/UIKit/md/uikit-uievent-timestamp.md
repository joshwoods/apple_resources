

- UIKit
- UIEvent
-  timestamp 

Instance Property

# timestamp

The time when the event occurred.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var timestamp: TimeInterval { get }
```

## Discussion

This property contains the number of seconds that have elapsed since system startup. For a description of this time value, see the description of the systemUptime method of the ProcessInfo class.

