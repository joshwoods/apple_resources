

- Core NFC
-  NFCNDEFStatus 

Enumeration

# NFCNDEFStatus

Constants that indicate status for an NDEF tag.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
enum NFCNDEFStatus
```

## Topics

### Statuses

case notSupported

A status indicating that that tag isn’t an NDEF-formatted tag.

case readOnly

A status indicating that the tag supports reading NDEF message data only.

case readWrite

A status indicating that the tag supports reading and writing NDEF message data.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting the Tag Status

var isAvailable: Bool

A Boolean value that determines whether the NDEF tag is available in the current reader session.

**Required**

func queryNDEFStatus(completionHandler: (NFCNDEFStatus, Int, (any Error)?) -> Void)

Asks the reader session for the NDEF support status of the tag.

**Required**

