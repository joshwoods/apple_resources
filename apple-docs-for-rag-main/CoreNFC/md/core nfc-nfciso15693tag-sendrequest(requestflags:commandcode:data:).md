

- Core NFC
- NFCISO15693Tag
-  sendRequest(requestFlags:commandCode:data:) 

Instance Method

# sendRequest(requestFlags:commandCode:data:)

iOS 14.0+iPadOS 14.0+Mac Catalyst

``` source
func sendRequest(
    requestFlags flags: Int,
    commandCode: Int,
    data: Data?
) async throws -> (NFCISO15693ResponseFlag, Data?)
```

