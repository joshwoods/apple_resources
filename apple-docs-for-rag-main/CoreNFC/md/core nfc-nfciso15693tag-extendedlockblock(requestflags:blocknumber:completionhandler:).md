

- Core NFC
- NFCISO15693Tag
-  extendedLockBlock(requestFlags:blockNumber:completionHandler:) 

Instance Method

# extendedLockBlock(requestFlags:blockNumber:completionHandler:)

Sends the Extended Lock Single Block command (0x32 command code), as defined in the NFC Forum Type 5 tag specification, to the tag.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
func extendedLockBlock(
    requestFlags flags: NFCISO15693RequestFlag,
    blockNumber: Int,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
func extendedLockBlock(
    requestFlags flags: NFCISO15693RequestFlag,
    blockNumber: Int
) async throws
```

**Required**

## See Also

### Sending Extended Commands

func extendedReadSingleBlock(requestFlags: NFCISO15693RequestFlag, blockNumber: Int, completionHandler: (Data, (any Error)?) -> Void)

Sends the Extended Read Single Block command (0x30 command code), as defined in the NFC Forum Type 5 tag specification, to the tag.

**Required**

func extendedWriteSingleBlock(requestFlags: NFCISO15693RequestFlag, blockNumber: Int, dataBlock: Data, completionHandler: ((any Error)?) -> Void)

Sends the Extended Write Single Block command (0x31 command code), as defined in the NFC Forum Type 5 tag specification, to the tag.

**Required**

func extendedReadMultipleBlocks(requestFlags: NFCISO15693RequestFlag, blockRange: NSRange, completionHandler: ([Data], (any Error)?) -> Void)

Sends the Extended Read Multiple Block command (0x33 command code), as defined in the NFC Forum Type 5 tag specification, to the tag.

**Required**

