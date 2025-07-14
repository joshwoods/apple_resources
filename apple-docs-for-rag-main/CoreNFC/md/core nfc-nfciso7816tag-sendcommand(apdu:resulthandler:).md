

- Core NFC
- NFCISO7816Tag
-  sendCommand(apdu:resultHandler:) 

Instance Method

# sendCommand(apdu:resultHandler:)

Sends an application protocol data unit (APDU) to the tag and receives a response APDU.

iOS 14.0+iPadOS 14.0+Mac Catalyst

``` source
func sendCommand(
    apdu: NFCISO7816APDU,
    resultHandler: @escaping (Result) -> Void
)
```

## Parameters 

`apdu`  

An application protocol data unit to send to the tag.

`resultHandler`  

A handler that the reader session invokes after the operation completes. The handler receives a Result with the cases:

`success`  
A instance of NFCISO7816ResponseAPDU containing the response from the tag.

`failure`  
An Error object indicating that a communication issue with the tag occurred.

## Discussion

When you send a `SELECT` command with a p1Parameter value of `0x04`, your app must support one of the applications listed in the com.apple.developer.nfc.readersession.iso7816.select-identifiers property list key. Otherwise, the `resultHandler` receives an NFCReaderError.Code.readerErrorSecurityViolation error.

The session calls `resultHandler` on the dispatch queue that you provided when creating the NFCTagReaderSession object.

## See Also

### Sending a Command

func sendCommand(apdu: NFCISO7816APDU, completionHandler: (Data, UInt8, UInt8, (any Error)?) -> Void)

Sends an application protocol data unit (APDU) to the tag and receives a response APDU.

**Required** Default implementation provided.

class NFCISO7816APDU

An object representing an ISO 7816 application protocol data unit (APDU).

struct NFCISO7816ResponseAPDU

An object containing the response from the tag.

