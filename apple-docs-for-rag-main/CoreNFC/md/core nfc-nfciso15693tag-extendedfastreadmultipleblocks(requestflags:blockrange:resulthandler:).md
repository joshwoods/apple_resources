

- Core NFC
- NFCISO15693Tag
-  extendedFastReadMultipleBlocks(requestFlags:blockRange:resultHandler:) 

Instance Method

# extendedFastReadMultipleBlocks(requestFlags:blockRange:resultHandler:)

iOS 14.0+iPadOS 14.0+Mac Catalyst

``` source
func extendedFastReadMultipleBlocks(
    requestFlags flags: NFCISO15693RequestFlag,
    blockRange: NSRange,
    resultHandler: @escaping (Result) -> Void
)
```

