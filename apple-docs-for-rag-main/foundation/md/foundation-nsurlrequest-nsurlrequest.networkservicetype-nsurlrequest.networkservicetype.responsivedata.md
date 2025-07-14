

- Foundation
- NSURLRequest
- NSURLRequest.NetworkServiceType
-  NSURLRequest.NetworkServiceType.responsiveData 

Case

# NSURLRequest.NetworkServiceType.responsiveData

A service type for medium-delay tolerant, elastic and inelastic flow, bursty, and long-lived connections.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case responsiveData
```

## Discussion

Use this service type for interactive situations where the user is anticipating a quick response, like instant messaging or completing a purchase.

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

case callSignaling

A service for low-loss tolerant, inelastic flow, jitter tolerant, short but bursty rate, and variable size connections.

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

case callSignaling

A service for low-loss tolerant, inelastic flow, jitter tolerant, short but bursty rate, and variable size connections.

case avStreaming

A service type for medium-delay tolerant, low-medium-loss tolerant, elastic flow, constant packet interval, and variable rate and size connections.

case responsiveAV

A service type for low-delay tolerant, low-to-medium-loss tolerant, elastic flow, variable packet interval, rate, size responsive and time-sensitive connections.

