

- CryptoTokenKit
- TKSmartCard
-  allowedProtocols 

Instance Property

# allowedProtocols

The protocols allowed for communication with the Smart Card. any by default.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var allowedProtocols: TKSmartCardProtocol { get set }
```

## Discussion

This property is consulted only when beginning a session to a Smart Card. Any changes to this property will not be reflected by the current session, if one is already established.

## See Also

### Setting the Communication Protocol

var currentProtocol: TKSmartCardProtocol

The protocol used for communication with the Smart Card. Returns TKSmartCardProtocolNone if no session is currently established.

struct TKSmartCardProtocol

Smart Card transmission protocols.

