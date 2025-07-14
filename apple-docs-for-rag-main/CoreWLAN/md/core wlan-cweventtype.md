

- Core WLAN
-  CWEventType 

Enumeration

# CWEventType

Wi-Fi event types.

macOS 10.10+

``` source
enum CWEventType
```

## Topics

### Constants

case none

No specified event type.

case powerDidChange

Posts when the power state of any Wi-Fi interface changes.

case ssidDidChange

Posts when the current SSID of any Wi-Fi interface changes.

case bssidDidChange

Posts when the current BSSID of any Wi-Fi interface changes.

case countryCodeDidChange

Posts when the adopted country code of any Wi-Fi interface changes.

case linkDidChange

Posts when the link state for any Wi-Fi interface changes.

case linkQualityDidChange

Posts when the RSSI or transmit rate for any Wi-Fi interface changes.

case modeDidChange

Posts when the operating mode of any Wi-Fi interface changes.

case scanCacheUpdated

Posts when the scan cache of any Wi-Fi interface is updated with new scan results.

case unknown

Unknown event type.

### Enumeration Cases

case btCoexStats

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

enum CWIBSSModeSecurity

IBSS mode security types.

Deprecated

enum CWInterfaceMode

Wi-Fi interface operating modes.

enum CWKeychainDomain

Keychain domain types that CoreWLAN keychain methods use.

enum CWPHYMode

CoreWLAN physical layer modes.

enum CWSecurity

CoreWLAN security types.

