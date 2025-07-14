

- CryptoTokenKit
- TKSmartCardATR
-  historicalRecords 

Instance Property

# historicalRecords

A list of compact TLV records parsed from historical bytes.

iOSiPadOSMac Catalyst 13.1+macOS 10.12+tvOSvisionOSwatchOS

``` source
var historicalRecords: [TKCompactTLVRecord]? { get }
```

## See Also

### Accessing ATR Attributes

var protocols: [NSNumber]

An array of protocols indicated in the ATR

var bytes: Data

The ATR message data.

var historicalBytes: Data

The ATR historical bytes, not including interface bytes or the TCK (check byte).

