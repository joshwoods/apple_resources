

- Core NFC
- NFCISO15693Tag
-  select(requestFlags:completionHandler:) 

Instance Method

# select(requestFlags:completionHandler:)

Sends the Select command (0x25 command code), as defined in the ISO 15693-3 specification, to the tag.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
func select(
    requestFlags flags: NFCISO15693RequestFlag,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
func select(requestFlags flags: NFCISO15693RequestFlag) async throws
```

**Required**

