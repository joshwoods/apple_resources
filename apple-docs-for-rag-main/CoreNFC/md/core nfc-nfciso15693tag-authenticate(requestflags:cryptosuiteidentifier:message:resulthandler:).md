

- Core NFC
- NFCISO15693Tag
-  authenticate(requestFlags:cryptoSuiteIdentifier:message:resultHandler:) 

Instance Method

# authenticate(requestFlags:cryptoSuiteIdentifier:message:resultHandler:)

iOS 14.0+iPadOS 14.0+Mac Catalyst

``` source
func authenticate(
    requestFlags flags: NFCISO15693RequestFlag,
    cryptoSuiteIdentifier: Int,
    message: Data,
    resultHandler: @escaping (Result) -> Void
)
```

