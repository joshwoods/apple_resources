

- Core NFC
- NFCISO15693Tag
-  writeAFI(requestFlags:afi:completionHandler:) 

Instance Method

# writeAFI(requestFlags:afi:completionHandler:)

Sends the Write AFI command (0x27 command code), as defined in the ISO 15693-3 specification, to the tag.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
func writeAFI(
    requestFlags flags: NFCISO15693RequestFlag,
    afi: UInt8,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
func writeAFI(
    requestFlags flags: NFCISO15693RequestFlag,
    afi: UInt8
) async throws
```

**Required**

## See Also

### Sending Application Family Identifier Commands

func lockAFI(requestFlags: NFCISO15693RequestFlag, completionHandler: ((any Error)?) -> Void)

Sends the Lock AFI command (0x28 command code), as defined in the ISO 15693-3 specification, to the tag.

**Required**

