

- System Configuration
- SCNetworkReachabilityFlags
-  connectionOnDemand 

Type Property

# connectionOnDemand

The specified node name or address can be reached using the current network configuration, but a connection must first be established.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.6+tvOSvisionOS 1.0+

``` source
static var connectionOnDemand: SCNetworkReachabilityFlags { get }
```

## Discussion

The connection will be established “On Demand” by the `CFSocketStream` programming interface (see CFStream Socket Additions for information on this). Other functions will not establish the connection.

## See Also

### Constants

static var transientConnection: SCNetworkReachabilityFlags

The specified node name or address can be reached via a transient connection, such as PPP.

static var reachable: SCNetworkReachabilityFlags

The specified node name or address can be reached using the current network configuration.

static var connectionRequired: SCNetworkReachabilityFlags

The specified node name or address can be reached using the current network configuration, but a connection must first be established. If this flag is set, the `kSCNetworkReachabilityFlagsConnectionOnTraffic` flag, `kSCNetworkReachabilityFlagsConnectionOnDemand` flag, or `kSCNetworkReachabilityFlagsIsWWAN` flag is also typically set to indicate the type of connection required. If the user must manually make the connection, the `kSCNetworkReachabilityFlagsInterventionRequired` flag is also set.

static var connectionOnTraffic: SCNetworkReachabilityFlags

The specified node name or address can be reached using the current network configuration, but a connection must first be established. Any traffic directed to the specified name or address will initiate the connection.

static var interventionRequired: SCNetworkReachabilityFlags

The specified node name or address can be reached using the current network configuration, but a connection must first be established.

static var isLocalAddress: SCNetworkReachabilityFlags

The specified node name or address is one that is associated with a network interface on the current system.

static var isDirect: SCNetworkReachabilityFlags

Network traffic to the specified node name or address will not go through a gateway, but is routed directly to one of the interfaces in the system.

static var isWWAN: SCNetworkReachabilityFlags

The specified node name or address can be reached via a cellular connection, such as EDGE or GPRS.

static var connectionAutomatic: SCNetworkReachabilityFlags

The specified node name or address can be reached using the current network configuration, but a connection must first be established. Any traffic directed to the specified name or address will initiate the connection. This flag is a synonym for connectionOnTraffic.

