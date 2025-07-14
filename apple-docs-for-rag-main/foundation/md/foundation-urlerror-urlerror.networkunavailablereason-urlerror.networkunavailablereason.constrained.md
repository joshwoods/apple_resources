

- Foundation
- URLError
- URLError.NetworkUnavailableReason
-  URLError.NetworkUnavailableReason.constrained 

Case

# URLError.NetworkUnavailableReason.constrained

A reason that indicates network is unavailable because the user enabled “Low Data Mode” in the Settings app.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
case constrained
```

## Discussion

This reason occurs when the following conditions are true:

- The only available network is cellular.

- The user has enabled “Low Data Mode” option in the Cellular Data Options section of the Settings app.

- The URLSessionConfiguration property allowsConstrainedNetworkAccess is false.

## See Also

### Unavailability reasons

case cellular

A reason that indicates network is unavailable because the interface is cellular and cellular network is disabled.

case expensive

A reason that indicates network is unavailable because the system marked the interface as expensive.

