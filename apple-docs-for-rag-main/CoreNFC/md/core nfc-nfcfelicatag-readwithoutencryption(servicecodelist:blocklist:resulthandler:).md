

- Core NFC
- NFCFeliCaTag
-  readWithoutEncryption(serviceCodeList:blockList:resultHandler:) 

Instance Method

# readWithoutEncryption(serviceCodeList:blockList:resultHandler:)

iOS 14.0+iPadOS 14.0+Mac Catalyst

``` source
func readWithoutEncryption(
    serviceCodeList: [Data],
    blockList: [Data],
    resultHandler: @escaping (Result) -> Void
)
```

