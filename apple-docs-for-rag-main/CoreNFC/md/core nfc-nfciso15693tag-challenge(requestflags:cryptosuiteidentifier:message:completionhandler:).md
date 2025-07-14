

- Core NFC
- NFCISO15693Tag
-  challenge(requestFlags:cryptoSuiteIdentifier:message:completionHandler:) 

Instance Method

# challenge(requestFlags:cryptoSuiteIdentifier:message:completionHandler:)

iOS 14.0+iPadOS 14.0+Mac Catalyst

``` source
func challenge(
    requestFlags flags: NFCISO15693RequestFlag,
    cryptoSuiteIdentifier: Int,
    message: Data,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

