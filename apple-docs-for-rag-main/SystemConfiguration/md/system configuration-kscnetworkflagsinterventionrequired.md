

- System Configuration
-  kSCNetworkFlagsInterventionRequired 

Global Variable

# kSCNetworkFlagsInterventionRequired

The specified node name or address can be reached using the current network configuration, but a connection must first be established.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var kSCNetworkFlagsInterventionRequired: Int { get }
```

## Discussion

In addition, some form of user intervention will be required to establish this connection, such as providing a password, an authentication token, etc.

Currently, this flag is returned when there is a dial-on-traffic configuration (`ConnectionAutomatic`), an attempt to connect has already been made, and when some error (for example, no dial tone, no answer, bad password, etc.) was encountered during the automatic connection attempt. In this case the PPP controller stops attempting to establish a connection until the user has intervened.

## See Also

### Constants

var kSCNetworkFlagsTransientConnection: Int

The specified node name or address can be reached via a transient connection, such as PPP.

var kSCNetworkFlagsReachable: Int

The specified node name or address can be reached using the current network configuration.

var kSCNetworkFlagsConnectionRequired: Int

The specified node name or address can be reached using the current network configuration, but a connection must first be established.

var kSCNetworkFlagsConnectionAutomatic: Int

The specified node name or address can be reached using the current network configuration, but a connection must first be established.

var kSCNetworkFlagsIsLocalAddress: Int

The specified node name or address is one associated with a network interface on the current system.

var kSCNetworkFlagsIsDirect: Int

Network traffic to the specified node name or address does not go through a gateway, but is routed directly to one of the interfaces in the system.

