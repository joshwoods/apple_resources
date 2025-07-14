

- Foundation
- NSURLRequest
- NSURLRequest.NetworkServiceType
-  NSURLRequest.NetworkServiceType.voip Deprecated

Case

# NSURLRequest.NetworkServiceType.voip

A service type for VoIP traffic.

iOS 4.0–13.0DeprecatediPadOS 4.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.7–10.15DeprecatedtvOS 9.0–13.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–6.0Deprecated

``` source
case voip
```

Deprecated

This service type has been depreciated, use service type NSURLRequest.NetworkServiceType.voice instead.

## Discussion

With the VoIP service type, the kernel continues to listen for incoming traffic while your app is in the background, then wakes up your app whenever new data arrives. Set this *only* for connections that are communicate with a VoIP service.

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

case responsiveData

A service type for medium-delay tolerant, elastic and inelastic flow, bursty, and long-lived connections.

case avStreaming

A service type for medium-delay tolerant, low-medium-loss tolerant, elastic flow, constant packet interval, and variable rate and size connections.

case responsiveAV

A service type for low-delay tolerant, low-to-medium-loss tolerant, elastic flow, variable packet interval, rate, size responsive and time-sensitive connections.

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

case responsiveData

A service type for medium-delay tolerant, elastic and inelastic flow, bursty, and long-lived connections.

case avStreaming

A service type for medium-delay tolerant, low-medium-loss tolerant, elastic flow, constant packet interval, and variable rate and size connections.

