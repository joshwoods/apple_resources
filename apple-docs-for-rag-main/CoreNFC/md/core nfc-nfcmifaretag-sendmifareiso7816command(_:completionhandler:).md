

- Core NFC
- NFCMiFareTag
-  sendMiFareISO7816Command(\_:completionHandler:) 

Instance Method

# sendMiFareISO7816Command(\_:completionHandler:)

Sends an ISO 7816 command APDU to the tag and receives a response APDU.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
func sendMiFareISO7816Command(
    _ apdu: NFCISO7816APDU,
    completionHandler: @escaping (Data, UInt8, UInt8, (any Error)?) -> Void
)
```

``` source
func sendMiFareISO7816Command(_ apdu: NFCISO7816APDU) async throws -> (Data, UInt8, UInt8)
```

**Required** Default implementation provided.

## Parameters 

`apdu`  

An ISO 7816-4 command APDU object.

`completionHandler`  

A handler that the reader session invokes after the operation completes. The session calls `completionHandler` on the dispatch queue that you provided when creating the NFCTagReaderSession object.

The handler has the following parameters:

responseData  
An NSData object containing the APDU response.

sw1  
The SW1 command-processing status byte.

sw2  
The SW2 command-processing status byte.

error  
`nil` when the operation is successful; otherwise, an NSError object indicating that a problem occurred while communicating with the tag, or that the tag doesn’t support ISO 7816-4 commands.

## Discussion

Use this method to send commands to tags that have a mifareFamily value of either NFCMiFareFamily.plus or NFCMiFareFamily.desfire.

## Default Implementations

### NFCMiFareTag Implementations

func sendMiFareISO7816Command(NFCISO7816APDU) async throws -> NFCISO7816ResponseAPDU

## See Also

### Sending Commands

func sendMiFareCommand(commandPacket: Data, completionHandler: (Data, (any Error)?) -> Void)

Sends a native MIFARE command to the tag.

**Required**

