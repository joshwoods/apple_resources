

- Matter
-  MTRThreadOperationalDataset 

Class

# MTRThreadOperationalDataset

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 16.1+visionOS 1.0+watchOS 9.1+

``` source
class MTRThreadOperationalDataset
```

## Topics

### Initializers

init?(data: Data)

init?(networkName: String, extendedPANID: Data, masterKey: Data, PSKc: Data, channel: UInt16, panID: Data)Deprecated

init?(networkName: String, extendedPANID: Data, masterKey: Data, psKc: Data, channelNumber: NSNumber, panID: Data)

### Instance Properties

var channel: UInt16Deprecated

var channelNumber: NSNumber

var extendedPANID: Data

var masterKey: Data

var networkName: String

var panID: Data

var psKc: Data

### Instance Methods

func data() -> Data

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

