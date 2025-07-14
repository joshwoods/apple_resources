

- System Configuration
-  kSCBondStatusNoPartner 

Global Variable

# kSCBondStatusNoPartner

The port on the switch to which the device is connected doesn’t seem to have 802.3ad Link Aggregation enabled.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var kSCBondStatusNoPartner: Int { get }
```

## See Also

### Constants

var kSCBondStatusOK: Int

The status is valid (for example, enabled, active, running, and so on).

var kSCBondStatusLinkInvalid: Int

The link state is not valid (such as down, half-duplex, or wrong speed).

var kSCBondStatusNotInActiveGroup: Int

Communication with a partner is occurring, but the link aggregation group is different from the one that is active.

var kSCBondStatusUnknown: Int

Nonspecific failure.

