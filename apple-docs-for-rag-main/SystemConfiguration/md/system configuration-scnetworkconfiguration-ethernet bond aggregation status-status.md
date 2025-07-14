

- System Configuration
- SCNetworkConfiguration
-  Ethernet Bond Aggregation Status 

API Collection

# Ethernet Bond Aggregation Status

Ethernet bond aggregation status codes.

## Topics

### Constants

var kSCBondStatusOK: Int

The status is valid (for example, enabled, active, running, and so on).

var kSCBondStatusLinkInvalid: Int

The link state is not valid (such as down, half-duplex, or wrong speed).

var kSCBondStatusNoPartner: Int

The port on the switch to which the device is connected doesn’t seem to have 802.3ad Link Aggregation enabled.

var kSCBondStatusNotInActiveGroup: Int

Communication with a partner is occurring, but the link aggregation group is different from the one that is active.

var kSCBondStatusUnknown: Int

Nonspecific failure.

## See Also

### Constants

Ethernet Bond Status Constants

Ethernet bond status codes.

Network Interface Types

Keys that identify network interface types.

Network Protocol Types

Keys that identify network protocol types.

