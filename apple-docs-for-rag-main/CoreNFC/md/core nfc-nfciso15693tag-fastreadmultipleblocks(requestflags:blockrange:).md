

- Core NFC
- NFCISO15693Tag
-  fastReadMultipleBlocks(requestFlags:blockRange:) 

Instance Method

# fastReadMultipleBlocks(requestFlags:blockRange:)

iOS 14.0+iPadOS 14.0+Mac Catalyst

``` source
func fastReadMultipleBlocks(
    requestFlags flags: NFCISO15693RequestFlag,
    blockRange: NSRange
) async throws -> [Data]
```

