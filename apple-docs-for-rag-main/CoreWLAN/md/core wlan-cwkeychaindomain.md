

- Core WLAN
-  CWKeychainDomain 

Enumeration

# CWKeychainDomain

Keychain domain types that CoreWLAN keychain methods use.

macOS 10.10+

``` source
enum CWKeychainDomain
```

## Topics

### Constants

case none

No keychain domain specified.

case user

The user keychain domain.

case system

The system keychain domain.

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

enum CWPHYMode

CoreWLAN physical layer modes.

enum CWSecurity

CoreWLAN security types.

