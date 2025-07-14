

- System Configuration
-  kSCNetworkFlagsTransientConnection 

Global Variable

# kSCNetworkFlagsTransientConnection

The specified node name or address can be reached via a transient connection, such as PPP.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var kSCNetworkFlagsTransientConnection: Int { get }
```

## See Also

### Constants

var kSCNetworkFlagsReachable: Int

The specified node name or address can be reached using the current network configuration.

var kSCNetworkFlagsConnectionRequired: Int

The specified node name or address can be reached using the current network configuration, but a connection must first be established.

var kSCNetworkFlagsConnectionAutomatic: Int

The specified node name or address can be reached using the current network configuration, but a connection must first be established.

var kSCNetworkFlagsInterventionRequired: Int

The specified node name or address can be reached using the current network configuration, but a connection must first be established.

var kSCNetworkFlagsIsLocalAddress: Int

The specified node name or address is one associated with a network interface on the current system.

var kSCNetworkFlagsIsDirect: Int

Network traffic to the specified node name or address does not go through a gateway, but is routed directly to one of the interfaces in the system.

