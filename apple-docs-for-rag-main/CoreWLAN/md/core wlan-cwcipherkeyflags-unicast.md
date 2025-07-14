

- Core WLAN
- CWCipherKeyFlags
-  unicast 

Type Property

# unicast

A flag that indicates to use the cipher key for unicast packets.

macOS 10.7+

``` source
static var unicast: CWCipherKeyFlags { get }
```

## See Also

### Constants

static var multicast: CWCipherKeyFlags

A flag that indicates to use the cipher key for multicast packets.

static var tx: CWCipherKeyFlags

A flag that indicates to use the cipher key for packets sent from the interface.

static var rx: CWCipherKeyFlags

A flag that indicates to use the cipher key for packets received by the interface.

