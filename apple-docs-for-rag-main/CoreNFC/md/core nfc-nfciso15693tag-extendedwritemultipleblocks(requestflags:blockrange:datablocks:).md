

- Core NFC
- NFCISO15693Tag
-  extendedWriteMultipleBlocks(requestFlags:blockRange:dataBlocks:) 

Instance Method

# extendedWriteMultipleBlocks(requestFlags:blockRange:dataBlocks:)

iOS 14.0+iPadOS 14.0+Mac Catalyst

``` source
func extendedWriteMultipleBlocks(
    requestFlags flags: NFCISO15693RequestFlag,
    blockRange: NSRange,
    dataBlocks: [Data]
) async throws
```

