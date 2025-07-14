

- Core NFC
- NFCISO15693Tag
-  sendRequest(requestFlags:commandCode:data:resultHandler:) 

Instance Method

# sendRequest(requestFlags:commandCode:data:resultHandler:)

iOS 14.0+iPadOS 14.0+Mac Catalyst

``` source
func sendRequest(
    requestFlags flags: Int,
    commandCode: Int,
    data: Data?,
    resultHandler: @escaping (Result) -> Void
)
```

