

- Core WLAN
-  CWInterfaceMode 

Enumeration

# CWInterfaceMode

Wi-Fi interface operating modes.

macOS 10.7+

``` source
enum CWInterfaceMode
```

## Topics

### Constants

case none

Interface is not in any mode.

case station

Interface is participating in an infrastructure network as a non-AP station.

case IBSS

Interface is participating in an IBSS network.

case hostAP

Interface is participating in an infrastructure network as an access point.

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

enum CWKeychainDomain

Keychain domain types that CoreWLAN keychain methods use.

enum CWPHYMode

CoreWLAN physical layer modes.

enum CWSecurity

CoreWLAN security types.

