

- Core WLAN
- CWCipherKeyFlags
-  multicast 

Type Property

# multicast

A flag that indicates to use the cipher key for multicast packets.

macOS 10.7+

``` source
static var multicast: CWCipherKeyFlags { get }
```

## See Also

### Constants

static var unicast: CWCipherKeyFlags

A flag that indicates to use the cipher key for unicast packets.

static var tx: CWCipherKeyFlags

A flag that indicates to use the cipher key for packets sent from the interface.

static var rx: CWCipherKeyFlags

A flag that indicates to use the cipher key for packets received by the interface.

