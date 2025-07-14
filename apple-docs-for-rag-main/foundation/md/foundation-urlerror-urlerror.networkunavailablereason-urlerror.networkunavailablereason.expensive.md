

- Foundation
- URLError
- URLError.NetworkUnavailableReason
-  URLError.NetworkUnavailableReason.expensive 

Case

# URLError.NetworkUnavailableReason.expensive

A reason that indicates network is unavailable because the system marked the interface as expensive.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
case expensive
```

## Discussion

The system determines what constitutes “expensive” based on the nature of the network interface and other factors. iOS 13 considers most cellular networks and personal hotspots expensive.

This reason occurs when the following conditions are true:

- The only available network interfaces are expensive.

- The URLSessionConfiguration property allowsExpensiveNetworkAccess is false.

## See Also

### Unavailability reasons

case cellular

A reason that indicates network is unavailable because the interface is cellular and cellular network is disabled.

case constrained

A reason that indicates network is unavailable because the user enabled “Low Data Mode” in the Settings app.

