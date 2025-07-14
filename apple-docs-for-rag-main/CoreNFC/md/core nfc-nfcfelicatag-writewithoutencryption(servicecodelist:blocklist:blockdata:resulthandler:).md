

- Core NFC
- NFCFeliCaTag
-  writeWithoutEncryption(serviceCodeList:blockList:blockData:resultHandler:) 

Instance Method

# writeWithoutEncryption(serviceCodeList:blockList:blockData:resultHandler:)

iOS 14.0+iPadOS 14.0+Mac Catalyst

``` source
func writeWithoutEncryption(
    serviceCodeList: [Data],
    blockList: [Data],
    blockData: [Data],
    resultHandler: @escaping (Result) -> Void
)
```

