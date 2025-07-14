

- Core NFC
- NFCISO7816Tag
-  sendCommand(apdu:completionHandler:) 

Instance Method

# sendCommand(apdu:completionHandler:)

Sends an application protocol data unit (APDU) to the tag and receives a response APDU.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
func sendCommand(
    apdu: NFCISO7816APDU,
    completionHandler: @escaping (Data, UInt8, UInt8, (any Error)?) -> Void
)
```

``` source
func sendCommand(apdu: NFCISO7816APDU) async throws -> (Data, UInt8, UInt8)
```

**Required** Default implementation provided.

## Parameters 

`apdu`  

An application protocol data unit to send to the tag.

`completionHandler`  

A handler that the reader session invokes after the operation completes. The handler has the following parameters:

responseData  
The response data, which may be empty even if the operation completes successfully.

sw1  
The SW1 command-processing status byte. This value is always valid.

sw2  
The SW2 command-processing status byte. This value is always valid.

error  
`nil` when the operation completes successfully; otherwise, an NSError object when there’s a communication issue with the tag.

## Discussion

When you send a `SELECT` command with a p1Parameter value of `0x04`, your app must support one of the applications listed in the com.apple.developer.nfc.readersession.iso7816.select-identifiers property list key. Otherwise, the `completionHandler` receives an NFCReaderError.Code.readerErrorSecurityViolation error.

The session calls `completionHandler` on the dispatch queue that you provided when creating the NFCTagReaderSession object.

## Default Implementations

### NFCISO7816Tag Implementations

func sendCommand(apdu: NFCISO7816APDU) async throws -> NFCISO7816ResponseAPDU

## See Also

### Sending a Command

func sendCommand(apdu: NFCISO7816APDU, resultHandler: (Result&lt;NFCISO7816ResponseAPDU, any Error>) -> Void)

Sends an application protocol data unit (APDU) to the tag and receives a response APDU.

class NFCISO7816APDU

An object representing an ISO 7816 application protocol data unit (APDU).

struct NFCISO7816ResponseAPDU

An object containing the response from the tag.

