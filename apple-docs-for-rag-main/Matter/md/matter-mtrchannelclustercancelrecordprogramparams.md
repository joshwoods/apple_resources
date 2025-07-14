

- Matter
-  MTRChannelClusterCancelRecordProgramParams 

Class

# MTRChannelClusterCancelRecordProgramParams

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
class MTRChannelClusterCancelRecordProgramParams
```

## Topics

### Instance Properties

var data: Data

var programIdentifier: String

var serverSideProcessingTimeout: NSNumber?

Controls how much time, in seconds, we will allow for the server to process the command.

var shouldRecordSeries: NSNumber

var timedInvokeTimeoutMs: NSNumber?

Controls whether the command is a timed command (using Timed Invoke).

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

