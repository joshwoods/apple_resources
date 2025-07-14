

- Core WLAN
-  CWPHYMode 

Enumeration

# CWPHYMode

CoreWLAN physical layer modes.

macOS 10.7+

``` source
enum CWPHYMode
```

## Topics

### Constants

case modeNone

No specified mode.

case mode11a

IEEE 802.11a PHY.

case mode11b

IEEE 802.11b PHY.

case mode11g

IEEE 802.11g PHY.

case mode11n

IEEE 802.11n PHY.

case mode11ac

IEEE 802.11ac PHY.

### Enumeration Cases

case mode11ax

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Enumerations

enum CWChannelBand

CoreWLAN channel bands.

enum CWChannelWidth

CoreWLAN channel widths.

struct CWCipherKeyFlags

Cipher key flags.

enum CWErr

enum CWEventType

Wi-Fi event types.

enum CWIBSSModeSecurity

IBSS mode security types.

Deprecated

enum CWInterfaceMode

Wi-Fi interface operating modes.

enum CWKeychainDomain

Keychain domain types that CoreWLAN keychain methods use.

enum CWSecurity

CoreWLAN security types.

