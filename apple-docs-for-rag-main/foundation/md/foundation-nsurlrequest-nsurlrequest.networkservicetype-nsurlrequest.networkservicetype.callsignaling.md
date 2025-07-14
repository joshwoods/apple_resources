

- Foundation
- NSURLRequest
- NSURLRequest.NetworkServiceType
-  NSURLRequest.NetworkServiceType.callSignaling 

Case

# NSURLRequest.NetworkServiceType.callSignaling

A service for low-loss tolerant, inelastic flow, jitter tolerant, short but bursty rate, and variable size connections.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
case callSignaling
```

## Discussion

Use this for establishing, maintaining, and tearing down a VoIP call.

## See Also

### Network service types

case `default`

A service type for standard network traffic.

case video

A service type for low-delay tolerant, very low-loss tolerant, inelastic flow, and constant packet rate connections.

case background

A service type for high-delay tolerant, high-loss tolerant, elastic flow, and variable size connections.

case voice

A service type for low-delay tolerant, very low-loss tolerant, inelastic flow, and constant packet rate connections.

case responsiveData

A service type for medium-delay tolerant, elastic and inelastic flow, bursty, and long-lived connections.

case avStreaming

A service type for medium-delay tolerant, low-medium-loss tolerant, elastic flow, constant packet interval, and variable rate and size connections.

case responsiveAV

A service type for low-delay tolerant, low-to-medium-loss tolerant, elastic flow, variable packet interval, rate, size responsive and time-sensitive connections.

case voip

A service type for VoIP traffic.

Deprecated

case `default`

A service type for standard network traffic.

case video

A service type for low-delay tolerant, very low-loss tolerant, inelastic flow, and constant packet rate connections.

case background

A service type for high-delay tolerant, high-loss tolerant, elastic flow, and variable size connections.

case voice

A service type for low-delay tolerant, very low-loss tolerant, inelastic flow, and constant packet rate connections.

case responsiveData

A service type for medium-delay tolerant, elastic and inelastic flow, bursty, and long-lived connections.

case avStreaming

A service type for medium-delay tolerant, low-medium-loss tolerant, elastic flow, constant packet interval, and variable rate and size connections.

case responsiveAV

A service type for low-delay tolerant, low-to-medium-loss tolerant, elastic flow, variable packet interval, rate, size responsive and time-sensitive connections.

