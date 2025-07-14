

- Core NFC
-  NFCISO7816ResponseAPDU 

Structure

# NFCISO7816ResponseAPDU

An object containing the response from the tag.

iOS 14.0+iPadOS 14.0+Mac Catalyst

``` source
struct NFCISO7816ResponseAPDU
```

## Topics

### Response Data

var payload: Data?

A data object that contains the response data.

var statusWord1: UInt8

The SW1 command-processing status byte.

var statusWord2: UInt8

The SW2 command-processing status byte.

## See Also

### Sending a Command

func sendCommand(apdu: NFCISO7816APDU, resultHandler: (Result&lt;NFCISO7816ResponseAPDU, any Error>) -> Void)

Sends an application protocol data unit (APDU) to the tag and receives a response APDU.

func sendCommand(apdu: NFCISO7816APDU, completionHandler: (Data, UInt8, UInt8, (any Error)?) -> Void)

Sends an application protocol data unit (APDU) to the tag and receives a response APDU.

**Required** Default implementation provided.

class NFCISO7816APDU

An object representing an ISO 7816 application protocol data unit (APDU).

