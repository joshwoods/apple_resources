

- Core NFC
- NFCNDEFTag
-  isAvailable 

Instance Property

# isAvailable

A Boolean value that determines whether the NDEF tag is available in the current reader session.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
var isAvailable: Bool { get }
```

**Required**

## Discussion

A tag removed from the RF field becomes unavailable, and a tag in a disconnected state is also unavailable.

## See Also

### Getting the Tag Status

func queryNDEFStatus(completionHandler: (NFCNDEFStatus, Int, (any Error)?) -> Void)

Asks the reader session for the NDEF support status of the tag.

**Required**

enum NFCNDEFStatus

Constants that indicate status for an NDEF tag.

