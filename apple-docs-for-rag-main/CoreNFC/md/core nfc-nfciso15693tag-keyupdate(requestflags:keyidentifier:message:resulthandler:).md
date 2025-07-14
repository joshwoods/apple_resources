

- Core NFC
- NFCISO15693Tag
-  keyUpdate(requestFlags:keyIdentifier:message:resultHandler:) 

Instance Method

# keyUpdate(requestFlags:keyIdentifier:message:resultHandler:)

iOS 14.0+iPadOS 14.0+Mac Catalyst

``` source
func keyUpdate(
    requestFlags flags: NFCISO15693RequestFlag,
    keyIdentifier: Int,
    message: Data,
    resultHandler: @escaping (Result) -> Void
)
```

