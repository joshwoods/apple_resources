

- Core NFC
-  NFCNDEFTag 

Protocol

# NFCNDEFTag

An interface for interacting with an NDEF tag.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
protocol NFCNDEFTag : NSCopying, NSSecureCoding, NSObjectProtocol
```

## Topics

### Getting the Tag Status

var isAvailable: Bool

A Boolean value that determines whether the NDEF tag is available in the current reader session.

**Required**

func queryNDEFStatus(completionHandler: (NFCNDEFStatus, Int, (any Error)?) -> Void)

Asks the reader session for the NDEF support status of the tag.

**Required**

enum NFCNDEFStatus

Constants that indicate status for an NDEF tag.

### Reading the Tag

func readNDEF(completionHandler: (NFCNDEFMessage?, (any Error)?) -> Void)

Retrieves an NDEF message from the tag.

**Required**

### Writing to the Tag

func writeNDEF(NFCNDEFMessage, completionHandler: ((any Error)?) -> Void)

Saves an NDEF message to a writable tag.

**Required**

func writeLock(completionHandler: ((any Error)?) -> Void)

Changes the NDEF tag status to read-only, preventing future write operations.

**Required**

## Relationships

### Inherits From

- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

### Inherited By

- NFCFeliCaTag
- NFCISO15693Tag
- NFCISO7816Tag
- NFCMiFareTag

## See Also

### Tag types

Creating NFC Tags from Your iPhone

Save data to tags, and interact with them using native tag protocols.

protocol NFCISO7816Tag

An interface for interacting with an ISO 7816 tag.

protocol NFCISO15693Tag

An interface for interacting with an ISO 15693 tag.

protocol NFCFeliCaTag

An interface for interacting with a FeliCa™ tag.

protocol NFCMiFareTag

An interface for interacting with a MIFARE® tag.

enum NFCTag

An object that represents an NFC tag object.

class NFCTagCommandConfiguration

A set of parameters you use to define the configuration of an NFC tag command.

