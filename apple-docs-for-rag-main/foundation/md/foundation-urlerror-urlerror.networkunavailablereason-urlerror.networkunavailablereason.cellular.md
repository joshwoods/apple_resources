

- Foundation
- URLError
- URLError.NetworkUnavailableReason
-  URLError.NetworkUnavailableReason.cellular 

Case

# URLError.NetworkUnavailableReason.cellular

A reason that indicates network is unavailable because the interface is cellular and cellular network is disabled.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
case cellular
```

## Discussion

This reason occurs when cellular is the only available network interface, but the URLSessionConfiguration property allowsCellularAccess is false.

## See Also

### Unavailability reasons

case constrained

A reason that indicates network is unavailable because the user enabled “Low Data Mode” in the Settings app.

case expensive

A reason that indicates network is unavailable because the system marked the interface as expensive.

