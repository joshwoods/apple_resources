

- Core NFC
- NFCISO15693Tag
-  authenticate(requestFlags:cryptoSuiteIdentifier:message:) 

Instance Method

# authenticate(requestFlags:cryptoSuiteIdentifier:message:)

iOS 14.0+iPadOS 14.0+Mac Catalyst

``` source
func authenticate(
    requestFlags flags: NFCISO15693RequestFlag,
    cryptoSuiteIdentifier: Int,
    message: Data
) async throws -> (NFCISO15693ResponseFlag, Data)
```

