

- CryptoTokenKit
-  TKSmartCardProtocol 

Structure

# TKSmartCardProtocol

Smart Card transmission protocols.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
struct TKSmartCardProtocol
```

## Topics

### Constants

static var t0: TKSmartCardProtocol

static var t1: TKSmartCardProtocol

static var t15: TKSmartCardProtocol

static var any: TKSmartCardProtocol

### Initializers

init(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Setting the Communication Protocol

var allowedProtocols: TKSmartCardProtocol

The protocols allowed for communication with the Smart Card. any by default.

var currentProtocol: TKSmartCardProtocol

The protocol used for communication with the Smart Card. Returns TKSmartCardProtocolNone if no session is currently established.

