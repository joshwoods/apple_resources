

- Core NFC
- NFCISO15693Tag
-  extendedFastReadMultipleBlocks(requestFlags:blockRange:) 

Instance Method

# extendedFastReadMultipleBlocks(requestFlags:blockRange:)

iOS 14.0+iPadOS 14.0+Mac Catalyst

``` source
func extendedFastReadMultipleBlocks(
    requestFlags flags: NFCISO15693RequestFlag,
    blockRange: NSRange
) async throws -> [Data]
```

