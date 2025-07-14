

- CryptoTokenKit
- TKSmartCard
-  currentProtocol 

Instance Property

# currentProtocol

The protocol used for communication with the Smart Card. Returns TKSmartCardProtocolNone if no session is currently established.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var currentProtocol: TKSmartCardProtocol { get }
```

## See Also

### Setting the Communication Protocol

var allowedProtocols: TKSmartCardProtocol

The protocols allowed for communication with the Smart Card. any by default.

struct TKSmartCardProtocol

Smart Card transmission protocols.

