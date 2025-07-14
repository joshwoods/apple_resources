

- Core NFC
- NFCISO15693Tag
-  readMultipleBlocks(requestFlags:blockRange:resultHandler:) 

Instance Method

# readMultipleBlocks(requestFlags:blockRange:resultHandler:)

iOS 14.0+iPadOS 14.0+Mac Catalyst

``` source
func readMultipleBlocks(
    requestFlags flags: NFCISO15693RequestFlag,
    blockRange: NSRange,
    resultHandler: @escaping (Result) -> Void
)
```

