

- Core NFC
- NFCISO7816ResponseAPDU
-  payload 

Instance Property

# payload

A data object that contains the response data.

iOS 14.0+iPadOS 14.0+Mac Catalyst

``` source
var payload: Data?
```

## Discussion

The data may be empty even if sendCommand(apdu:resultHandler:) completes successfully.

## See Also

### Response Data

var statusWord1: UInt8

The SW1 command-processing status byte.

var statusWord2: UInt8

The SW2 command-processing status byte.

