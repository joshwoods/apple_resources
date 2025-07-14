

- Core NFC
- NFCNDEFStatus
-  NFCNDEFStatus.notSupported 

Case

# NFCNDEFStatus.notSupported

A status indicating that that tag isn’t an NDEF-formatted tag.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
case notSupported
```

## Discussion

You cannot perform read and write operations on the tag.

## See Also

### Statuses

case readOnly

A status indicating that the tag supports reading NDEF message data only.

case readWrite

A status indicating that the tag supports reading and writing NDEF message data.

