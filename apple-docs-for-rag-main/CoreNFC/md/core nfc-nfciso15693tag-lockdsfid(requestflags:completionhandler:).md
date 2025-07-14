

- Core NFC
- NFCISO15693Tag
-  lockDSFID(requestFlags:completionHandler:) 

Instance Method

# lockDSFID(requestFlags:completionHandler:)

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
func lockDSFID(
    requestFlags flags: NFCISO15693RequestFlag,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
func lockDSFID(requestFlags flags: NFCISO15693RequestFlag) async throws
```

**Required**

