

- Core WLAN
-  CWSecurity 

Enumeration

# CWSecurity

CoreWLAN security types.

macOS 10.7+

``` source
enum CWSecurity
```

## Topics

### Constants

case none

Open System authentication.

case WEP

WEP security.

case wpaPersonal

WPA Personal authentication.

case wpaPersonalMixed

WPA/WPA2 Personal authentication.

case wpa2Personal

WPA2 Personal authentication.

case personal

Personal authentication.

case dynamicWEP

Dynamic WEP security.

case wpaEnterprise

WPA Enterprise authentication.

case wpaEnterpriseMixed

WPA/WPA2 Enterprise authentication.

case wpa2Enterprise

WPA2 Enterprise authentication.

case enterprise

Enterprise authentication.

case wpa3Personal

WPA3 Personal authentication.

case wpa3Enterprise

WPA3 Enterprise authentication.

case wpa3Transition

WPA3 Transition (WPA3/WPA2 Personal) authentication.

case unknown

Unknown security type.

### Enumeration Cases

case OWE

case oweTransition

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

enum CWPHYMode

CoreWLAN physical layer modes.

