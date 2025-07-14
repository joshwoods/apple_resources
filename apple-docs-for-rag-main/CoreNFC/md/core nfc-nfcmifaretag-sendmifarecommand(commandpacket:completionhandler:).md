

- Core NFC
- NFCMiFareTag
-  sendMiFareCommand(commandPacket:completionHandler:) 

Instance Method

# sendMiFareCommand(commandPacket:completionHandler:)

Sends a native MIFARE command to the tag.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
func sendMiFareCommand(
    commandPacket command: Data,
    completionHandler: @escaping (Data, (any Error)?) -> Void
)
```

``` source
func sendMiFareCommand(commandPacket command: Data) async throws -> Data
```

**Required**

## Parameters 

`command`  

A MIFARE command. For NFCMiFareFamily.ultralight commands, you must calculate a 2-byte CRC value and append it to the end of the `command` data.

`completionHandler`  

A handler that the reader session invokes after the operation completes. The session calls `completionHandler` on the dispatch queue that you provided when creating the NFCTagReaderSession object.

The handler has the following parameters:

response  
An NSData object containing the tag’s response data for the command.

error  
`nil` when the operation is successful; otherwise, an NSError object indicating that a problem occurred while communicating with the tag.

## Discussion

Use this method to send commands to tags that are from the NFCMiFareFamily.ultralight, NFCMiFareFamily.plus, and NFCMiFareFamily.desfire product families.

This method supports command chaining, passing the full response composed of the individual fragments to the `completionHandler`.

Note

This method doesn’t support the Crypto1 protocol.

## See Also

### Sending Commands

func sendMiFareISO7816Command(NFCISO7816APDU, completionHandler: (Data, UInt8, UInt8, (any Error)?) -> Void)

Sends an ISO 7816 command APDU to the tag and receives a response APDU.

**Required** Default implementation provided.

