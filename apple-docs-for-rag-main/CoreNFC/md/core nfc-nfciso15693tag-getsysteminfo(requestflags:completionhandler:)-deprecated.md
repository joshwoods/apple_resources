

- Core NFC
- NFCISO15693Tag
-  getSystemInfo(requestFlags:completionHandler:) Deprecated

Instance Method

# getSystemInfo(requestFlags:completionHandler:)

Sends the Get System Information command (0x2B command code), as defined in the ISO 15693-3 specification, to the tag.

iOS 13.0–14.0DeprecatediPadOS 13.0–14.0DeprecatedMac Catalyst 13.1–14.0Deprecated

``` source
func getSystemInfo(
    requestFlags flags: NFCISO15693RequestFlag,
    completionHandler: @escaping (Int, Int, Int, Int, Int, (any Error)?) -> Void
)
```

**Required**

