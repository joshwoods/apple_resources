

- Core NFC
- NFCISO15693Tag
-  readSingleBlock(requestFlags:blockNumber:resultHandler:) 

Instance Method

# readSingleBlock(requestFlags:blockNumber:resultHandler:)

iOS 14.0+iPadOS 14.0+Mac Catalyst

``` source
func readSingleBlock(
    requestFlags flags: NFCISO15693RequestFlag,
    blockNumber: UInt8,
    resultHandler: @escaping (Result) -> Void
)
```

