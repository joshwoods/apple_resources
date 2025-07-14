

- Core NFC
-  NFCVASCommandConfiguration 

Class

# NFCVASCommandConfiguration

An object providing the configuration for a GET VAS DATA command.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
class NFCVASCommandConfiguration
```

## Topics

### Creating a Command Configuration

init(vasMode: NFCVASCommandConfiguration.Mode, passTypeIdentifier: String, url: URL?)

Creates a VAS command configuration object.

### Setting Configuration Items

var mode: NFCVASCommandConfiguration.Mode

A VAS protocol mode.

typealias VASMode

Constants that indicate the VAS protocol mode.

Deprecated

var passTypeIdentifier: String

A type identifier for the Wallet Pass.

var url: URL?

A merchant URL.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Creating a VAS Reader Session

init(vasCommandConfigurations: [NFCVASCommandConfiguration], delegate: any NFCVASReaderSessionDelegate, queue: dispatch_queue_t?)

Creates a VAS reader session.

protocol NFCVASReaderSessionDelegate

A protocol that an object implements to receive callbacks from a VAS reader session.

