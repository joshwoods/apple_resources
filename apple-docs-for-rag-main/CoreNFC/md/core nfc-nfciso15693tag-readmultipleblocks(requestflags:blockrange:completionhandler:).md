

- Core NFC
- NFCISO15693Tag
-  readMultipleBlocks(requestFlags:blockRange:completionHandler:) 

Instance Method

# readMultipleBlocks(requestFlags:blockRange:completionHandler:)

Sends the Read Multiple Blocks command (0x23 command code), as defined in the ISO 15693-3 specification, to the tag.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
func readMultipleBlocks(
    requestFlags flags: NFCISO15693RequestFlag,
    blockRange: NSRange,
    completionHandler: @escaping ([Data], (any Error)?) -> Void
)
```

``` source
func readMultipleBlocks(
    requestFlags flags: NFCISO15693RequestFlag,
    blockRange: NSRange
) async throws -> [Data]
```

**Required**

## See Also

### Sending Multi-block Commands

func writeMultipleBlocks(requestFlags: NFCISO15693RequestFlag, blockRange: NSRange, dataBlocks: [Data], completionHandler: ((any Error)?) -> Void)

Sends the Write Multiple Blocks command (0x24 command code), as defined in the ISO 15693-3 specification, to the tag.

**Required**

func getMultipleBlockSecurityStatus(requestFlags: NFCISO15693RequestFlag, blockRange: NSRange, completionHandler: ([NSNumber], (any Error)?) -> Void)

Sends the Get Multiple Block Security Status command (0x2C command code), as defined in the ISO 15693-3 specification, to the tag.

**Required**

