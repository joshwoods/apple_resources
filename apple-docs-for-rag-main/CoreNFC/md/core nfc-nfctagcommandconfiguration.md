

- Core NFC
-  NFCTagCommandConfiguration 

Class

# NFCTagCommandConfiguration

A set of parameters you use to define the configuration of an NFC tag command.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
class NFCTagCommandConfiguration
```

## Topics

### Configuring a Tag Command

var maximumRetries: Int

The maximum number of retries.

var retryInterval: TimeInterval

The time between retries, in seconds.

## Relationships

### Inherits From

- NSObject

### Inherited By

- NFCISO15693CustomCommandConfiguration
- NFCISO15693ReadMultipleBlocksConfiguration

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

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

protocol NFCNDEFTag

An interface for interacting with an NDEF tag.

enum NFCTag

An object that represents an NFC tag object.

