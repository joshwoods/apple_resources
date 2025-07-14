

- Foundation
- URLSessionConfiguration
- URLSessionConfiguration.MultipathServiceType
-  URLSessionConfiguration.MultipathServiceType.interactive 

Case

# URLSessionConfiguration.MultipathServiceType.interactive

A service whereby Multipath TCP attempts to use the lowest-latency interface.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
case interactive
```

## Discussion

Specify this option for latency-sensitive, low-volume connections that might use cellular data. You must also set the Multipath Entitlement in the Xcode Capabilities pane for your app.

## See Also

### Service types

case none

The default service type indicating that Multipath TCP should not be used.

case handover

A Multipath TCP service that provides seamless handover between Wi-Fi and cellular in order to preserve the connection.

case aggregate

A service that aggregates the capacities of other Multipath options in an attempt to increase throughput and minimize latency.

