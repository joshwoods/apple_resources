

- CryptoTokenKit
- TKSmartCardATR
-  historicalBytes 

Instance Property

# historicalBytes

The ATR historical bytes, not including interface bytes or the TCK (check byte).

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var historicalBytes: Data { get }
```

## See Also

### Accessing ATR Attributes

var protocols: [NSNumber]

An array of protocols indicated in the ATR

var bytes: Data

The ATR message data.

var historicalRecords: [TKCompactTLVRecord]?

A list of compact TLV records parsed from historical bytes.

