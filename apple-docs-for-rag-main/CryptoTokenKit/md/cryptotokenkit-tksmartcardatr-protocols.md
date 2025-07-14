

- CryptoTokenKit
- TKSmartCardATR
-  protocols 

Instance Property

# protocols

An array of protocols indicated in the ATR

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var protocols: [NSNumber] { get }
```

## Discussion

Each element in the returned array is an `NSNumber` object containing an `NSUInteger` value corresponding to a member of the TKSmartCardProtocol enumeration.

The returned protocols are ordered such that the default protocol is at index `0`, and any duplicate values are removed.

## See Also

### Accessing ATR Attributes

var bytes: Data

The ATR message data.

var historicalBytes: Data

The ATR historical bytes, not including interface bytes or the TCK (check byte).

var historicalRecords: [TKCompactTLVRecord]?

A list of compact TLV records parsed from historical bytes.

