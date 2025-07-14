

- Core NFC
- NFCISO15693Tag
-  writeSingleBlock(requestFlags:blockNumber:dataBlock:completionHandler:) 

Instance Method

# writeSingleBlock(requestFlags:blockNumber:dataBlock:completionHandler:)

Sends the Write Single Block command (0x21 command code), as defined in the ISO 15693-3 specification, to the tag.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
func writeSingleBlock(
    requestFlags flags: NFCISO15693RequestFlag,
    blockNumber: UInt8,
    dataBlock: Data,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
func writeSingleBlock(
    requestFlags flags: NFCISO15693RequestFlag,
    blockNumber: UInt8,
    dataBlock: Data
) async throws
```

**Required**

## See Also

### Sending Single Block Commands

func readSingleBlock(requestFlags: NFCISO15693RequestFlag, blockNumber: UInt8, completionHandler: (Data, (any Error)?) -> Void)

Sends a Read Single Block command (0x20 command code), as defined in the ISO 15693-3 specification, to the tag.

**Required**

func lockBlock(requestFlags: NFCISO15693RequestFlag, blockNumber: UInt8, completionHandler: ((any Error)?) -> Void)

Sends the Lock Block command (0x22 command code), as defined in the ISO 15693-3 specification, to the tag.

**Required**

