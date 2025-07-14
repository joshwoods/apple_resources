

- Core NFC
- NFCISO7816ResponseAPDU
-  statusWord2 

Instance Property

# statusWord2

The SW2 command-processing status byte.

iOS 14.0+iPadOS 14.0+Mac Catalyst

``` source
var statusWord2: UInt8
```

## Discussion

This value is always valid.

## See Also

### Response Data

var payload: Data?

A data object that contains the response data.

var statusWord1: UInt8

The SW1 command-processing status byte.

