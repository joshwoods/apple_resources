

- CryptoTokenKit
- TKSmartCardATR
-  bytes 

Instance Property

# bytes

The ATR message data.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var bytes: Data { get }
```

## See Also

### Accessing ATR Attributes

var protocols: [NSNumber]

An array of protocols indicated in the ATR

var historicalBytes: Data

The ATR historical bytes, not including interface bytes or the TCK (check byte).

var historicalRecords: [TKCompactTLVRecord]?

A list of compact TLV records parsed from historical bytes.

