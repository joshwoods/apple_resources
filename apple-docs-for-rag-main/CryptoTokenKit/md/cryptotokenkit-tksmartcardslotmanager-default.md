

- CryptoTokenKit
- TKSmartCardSlotManager
-  default 

Type Property

# default

The shared singleton Smart Card reader slot manager.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
class var `default`: TKSmartCardSlotManager? { get }
```

## Discussion

This method returns `nil` unless the com.apple.security.smartcard entitlement is enabled.

