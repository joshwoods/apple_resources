

- Core NFC
- NFCISO15693Tag
-  customCommand(requestFlags:customCommandCode:customRequestParameters:resultHandler:) 

Instance Method

# customCommand(requestFlags:customCommandCode:customRequestParameters:resultHandler:)

iOS 14.0+iPadOS 14.0+Mac Catalyst

``` source
func customCommand(
    requestFlags flags: NFCISO15693RequestFlag,
    customCommandCode: Int,
    customRequestParameters: Data,
    resultHandler: @escaping (Result) -> Void
)
```

