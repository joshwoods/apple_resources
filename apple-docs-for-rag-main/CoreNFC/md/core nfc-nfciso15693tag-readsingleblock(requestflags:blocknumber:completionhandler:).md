

- Core NFC
- NFCISO15693Tag
-  readSingleBlock(requestFlags:blockNumber:completionHandler:) 

Instance Method

# readSingleBlock(requestFlags:blockNumber:completionHandler:)

Sends a Read Single Block command (0x20 command code), as defined in the ISO 15693-3 specification, to the tag.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
func readSingleBlock(
    requestFlags flags: NFCISO15693RequestFlag,
    blockNumber: UInt8,
    completionHandler: @escaping (Data, (any Error)?) -> Void
)
```

``` source
func readSingleBlock(
    requestFlags flags: NFCISO15693RequestFlag,
    blockNumber: UInt8
) async throws -> Data
```

**Required**

## Parameters 

`flags`  

The request flags. The RequestFlagAddress flag is enforced by default. However, using the RequestFlagSelect flag disables the RequestFlagAddress flag.

`blockNumber`  

The number of the block to read. Blocks are numbered from 0 to 255 inclusively.

`completionHandler`  

A handler that the reader session invokes after the operation completes. The session calls completionHandler on the dispatch queue that you provided when creating the NFCTagReaderSession object.

The handler has the following parameters:

data  
A NSData object containing the blocks of data read from the tag. If the request flags include RequestFlagOption, the first byte of the data contains the associated block security status.

error  
`nil` when the operation is successful; otherwise, an NSError object indicating that a problem occurred while communicating with the tag.

When the tag responds with a command error, the error’s userInfo directory contains the NFCISO15693TagResponseErrorKey and the error’s code property has a value defined in the ISO15693-3 specification.

## Discussion

This method sends the tag’s identifier with the command.

## See Also

### Sending Single Block Commands

func writeSingleBlock(requestFlags: NFCISO15693RequestFlag, blockNumber: UInt8, dataBlock: Data, completionHandler: ((any Error)?) -> Void)

Sends the Write Single Block command (0x21 command code), as defined in the ISO 15693-3 specification, to the tag.

**Required**

func lockBlock(requestFlags: NFCISO15693RequestFlag, blockNumber: UInt8, completionHandler: ((any Error)?) -> Void)

Sends the Lock Block command (0x22 command code), as defined in the ISO 15693-3 specification, to the tag.

**Required**

