

- System Configuration
- SCNetworkReachabilityFlags
-  isWWAN 

Type Property

# isWWAN

The specified node name or address can be reached via a cellular connection, such as EDGE or GPRS.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
static var isWWAN: SCNetworkReachabilityFlags { get }
```

## Discussion

Important

This absence of this flag does not necessarily mean that a connection will never pass over a cellular network. If you need to robustly prevent cellular networking, read Avoiding Common Networking Mistakes in Networking Overview.

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

static var connectionOnDemand: SCNetworkReachabilityFlags

The specified node name or address can be reached using the current network configuration, but a connection must first be established.

static var isLocalAddress: SCNetworkReachabilityFlags

The specified node name or address is one that is associated with a network interface on the current system.

static var isDirect: SCNetworkReachabilityFlags

Network traffic to the specified node name or address will not go through a gateway, but is routed directly to one of the interfaces in the system.

static var connectionAutomatic: SCNetworkReachabilityFlags

The specified node name or address can be reached using the current network configuration, but a connection must first be established. Any traffic directed to the specified name or address will initiate the connection. This flag is a synonym for connectionOnTraffic.

