

- Core NFC
- NFCISO15693Tag
-  fastReadMultipleBlocks(requestFlags:blockRange:resultHandler:) 

Instance Method

# fastReadMultipleBlocks(requestFlags:blockRange:resultHandler:)

iOS 14.0+iPadOS 14.0+Mac Catalyst

``` source
func fastReadMultipleBlocks(
    requestFlags flags: NFCISO15693RequestFlag,
    blockRange: NSRange,
    resultHandler: @escaping (Result) -> Void
)
```

