

- Foundation
- URLSessionConfiguration
- URLSessionConfiguration.MultipathServiceType
-  URLSessionConfiguration.MultipathServiceType.aggregate 

Case

# URLSessionConfiguration.MultipathServiceType.aggregate

A service that aggregates the capacities of other Multipath options in an attempt to increase throughput and minimize latency.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
case aggregate
```

## Discussion

This option is available only for experimentation. Specify it for connections that use cellular data. You must also set the Multipath Entitlement in the Xcode Capabilities pane for your app.

To enable the aggregation mode, open the Settings app on your development iPhone and navigate to Developer, and then turn on Multipath Networking.

Multipath Aggregation requires an iOS device in Developer mode with a cellular connection running iOS 11.0 or later.

Note

Setting this option will use a considerable amount of cellular data.

## See Also

### Service types

case none

The default service type indicating that Multipath TCP should not be used.

case handover

A Multipath TCP service that provides seamless handover between Wi-Fi and cellular in order to preserve the connection.

case interactive

A service whereby Multipath TCP attempts to use the lowest-latency interface.

