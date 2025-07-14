

- Core NFC
- NFCISO15693Tag
-  keyUpdate(requestFlags:keyIdentifier:message:) 

Instance Method

# keyUpdate(requestFlags:keyIdentifier:message:)

iOS 14.0+iPadOS 14.0+Mac Catalyst

``` source
func keyUpdate(
    requestFlags flags: NFCISO15693RequestFlag,
    keyIdentifier: Int,
    message: Data
) async throws -> (NFCISO15693ResponseFlag, Data)
```

