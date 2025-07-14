

- Core WLAN
- CWCipherKeyFlags
-  tx 

Type Property

# tx

A flag that indicates to use the cipher key for packets sent from the interface.

macOS 10.7+

``` source
static var tx: CWCipherKeyFlags { get }
```

## See Also

### Constants

static var unicast: CWCipherKeyFlags

A flag that indicates to use the cipher key for unicast packets.

static var multicast: CWCipherKeyFlags

A flag that indicates to use the cipher key for multicast packets.

static var rx: CWCipherKeyFlags

A flag that indicates to use the cipher key for packets received by the interface.

