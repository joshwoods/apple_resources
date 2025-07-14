

- System Configuration
-  kSCBondStatusNotInActiveGroup 

Global Variable

# kSCBondStatusNotInActiveGroup

Communication with a partner is occurring, but the link aggregation group is different from the one that is active.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var kSCBondStatusNotInActiveGroup: Int { get }
```

## See Also

### Constants

var kSCBondStatusOK: Int

The status is valid (for example, enabled, active, running, and so on).

var kSCBondStatusLinkInvalid: Int

The link state is not valid (such as down, half-duplex, or wrong speed).

var kSCBondStatusNoPartner: Int

The port on the switch to which the device is connected doesn’t seem to have 802.3ad Link Aggregation enabled.

var kSCBondStatusUnknown: Int

Nonspecific failure.

