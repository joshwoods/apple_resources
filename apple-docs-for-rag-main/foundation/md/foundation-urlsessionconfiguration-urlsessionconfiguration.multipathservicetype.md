

- Foundation
- URLSessionConfiguration
-  URLSessionConfiguration.MultipathServiceType 

Enumeration

# URLSessionConfiguration.MultipathServiceType

Constants that specify the type of service that Multipath TCP uses.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
enum MultipathServiceType
```

## Mentioned in 

Improving network reliability using Multipath TCP

## Topics

### Service types

case none

The default service type indicating that Multipath TCP should not be used.

case handover

A Multipath TCP service that provides seamless handover between Wi-Fi and cellular in order to preserve the connection.

case interactive

A service whereby Multipath TCP attempts to use the lowest-latency interface.

case aggregate

A service that aggregates the capacities of other Multipath options in an attempt to increase throughput and minimize latency.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Supporting Multipath TCP

Improving network reliability using Multipath TCP

Use the available radios in iOS devices to improve your app’s network reliability and performance.

var multipathServiceType: URLSessionConfiguration.MultipathServiceType

A service type that specifies the Multipath TCP connection policy for transmitting data over Wi-Fi and cellular interfaces.

Multipath Entitlement

A Boolean value indicating whether your app may use Multipath protocols to seamlessly transition between Wi-Fi and cellular networks.

