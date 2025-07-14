

- Foundation
- URLSessionConfiguration
- URLSessionConfiguration.MultipathServiceType
-  URLSessionConfiguration.MultipathServiceType.none 

Case

# URLSessionConfiguration.MultipathServiceType.none

The default service type indicating that Multipath TCP should not be used.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
case none
```

## See Also

### Service types

case handover

A Multipath TCP service that provides seamless handover between Wi-Fi and cellular in order to preserve the connection.

case interactive

A service whereby Multipath TCP attempts to use the lowest-latency interface.

case aggregate

A service that aggregates the capacities of other Multipath options in an attempt to increase throughput and minimize latency.

