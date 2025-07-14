

- System Configuration
- SCNetworkReachabilityFlags
-  interventionRequired 

Type Property

# interventionRequired

The specified node name or address can be reached using the current network configuration, but a connection must first be established.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
static var interventionRequired: SCNetworkReachabilityFlags { get }
```

## Discussion

In addition, some form of user intervention will be required to establish this connection, such as providing a password, an authentication token, etc.

Currently, this flag is returned only when there is a dial-on-traffic configuration (`kSCNetworkReachabilityFlagsConnectionOnTraffic`), an attempt to connect has already been made, and when some error (such as no dial tone, no answer, bad password, etc.) occurred during the automatic connection attempt. In this case the PPP controller stops attempting to establish a connection until the user has intervened.

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

static var connectionOnDemand: SCNetworkReachabilityFlags

The specified node name or address can be reached using the current network configuration, but a connection must first be established.

static var isLocalAddress: SCNetworkReachabilityFlags

The specified node name or address is one that is associated with a network interface on the current system.

static var isDirect: SCNetworkReachabilityFlags

Network traffic to the specified node name or address will not go through a gateway, but is routed directly to one of the interfaces in the system.

static var isWWAN: SCNetworkReachabilityFlags

The specified node name or address can be reached via a cellular connection, such as EDGE or GPRS.

static var connectionAutomatic: SCNetworkReachabilityFlags

The specified node name or address can be reached using the current network configuration, but a connection must first be established. Any traffic directed to the specified name or address will initiate the connection. This flag is a synonym for connectionOnTraffic.

