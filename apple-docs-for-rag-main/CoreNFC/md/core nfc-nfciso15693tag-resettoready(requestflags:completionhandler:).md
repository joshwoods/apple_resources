

- Core NFC
- NFCISO15693Tag
-  resetToReady(requestFlags:completionHandler:) 

Instance Method

# resetToReady(requestFlags:completionHandler:)

Sends the Reset To Ready command (0x26 command code), as defined in the ISO 15693-3 specification, to the tag.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
func resetToReady(
    requestFlags flags: NFCISO15693RequestFlag,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
func resetToReady(requestFlags flags: NFCISO15693RequestFlag) async throws
```

**Required**

