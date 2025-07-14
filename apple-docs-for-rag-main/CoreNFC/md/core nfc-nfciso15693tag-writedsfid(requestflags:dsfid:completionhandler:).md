

- Core NFC
- NFCISO15693Tag
-  writeDSFID(requestFlags:dsfid:completionHandler:) 

Instance Method

# writeDSFID(requestFlags:dsfid:completionHandler:)

Sends the Write DSFID command (0x29 command code), as defined in the ISO 15693-3 specification, to the tag.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
func writeDSFID(
    requestFlags flags: NFCISO15693RequestFlag,
    dsfid: UInt8,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
func writeDSFID(
    requestFlags flags: NFCISO15693RequestFlag,
    dsfid: UInt8
) async throws
```

**Required**

## See Also

### Sending Data Storage Format Identifier Commands

func lockDFSID(requestFlags: NFCISO15693RequestFlag, completionHandler: ((any Error)?) -> Void)

Sends the Lock DSFID command (0x2A command code), as defined in the ISO 15693-3 specification, to the tag.

**Required**

Deprecated

