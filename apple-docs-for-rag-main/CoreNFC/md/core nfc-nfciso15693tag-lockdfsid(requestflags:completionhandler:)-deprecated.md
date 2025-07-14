

- Core NFC
- NFCISO15693Tag
-  lockDFSID(requestFlags:completionHandler:) Deprecated

Instance Method

# lockDFSID(requestFlags:completionHandler:)

Sends the Lock DSFID command (0x2A command code), as defined in the ISO 15693-3 specification, to the tag.

iOS 13.0–14.0DeprecatediPadOS 13.0–14.0DeprecatedMac Catalyst 13.1–14.0Deprecated

``` source
func lockDFSID(
    requestFlags flags: NFCISO15693RequestFlag,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

**Required**

## See Also

### Sending Data Storage Format Identifier Commands

func writeDSFID(requestFlags: NFCISO15693RequestFlag, dsfid: UInt8, completionHandler: ((any Error)?) -> Void)

Sends the Write DSFID command (0x29 command code), as defined in the ISO 15693-3 specification, to the tag.

**Required**

