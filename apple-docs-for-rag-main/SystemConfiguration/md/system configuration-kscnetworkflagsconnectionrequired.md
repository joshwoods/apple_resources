

- System Configuration
-  kSCNetworkFlagsConnectionRequired 

Global Variable

# kSCNetworkFlagsConnectionRequired

The specified node name or address can be reached using the current network configuration, but a connection must first be established.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var kSCNetworkFlagsConnectionRequired: Int { get }
```

## Discussion

For example, this status would be returned for a dialup connection that was not currently active, but could handle network traffic for the target system.

## See Also

### Constants

var kSCNetworkFlagsTransientConnection: Int

The specified node name or address can be reached via a transient connection, such as PPP.

var kSCNetworkFlagsReachable: Int

The specified node name or address can be reached using the current network configuration.

var kSCNetworkFlagsConnectionAutomatic: Int

The specified node name or address can be reached using the current network configuration, but a connection must first be established.

var kSCNetworkFlagsInterventionRequired: Int

The specified node name or address can be reached using the current network configuration, but a connection must first be established.

var kSCNetworkFlagsIsLocalAddress: Int

The specified node name or address is one associated with a network interface on the current system.

var kSCNetworkFlagsIsDirect: Int

Network traffic to the specified node name or address does not go through a gateway, but is routed directly to one of the interfaces in the system.

