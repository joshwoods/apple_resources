

- Matter
-  MTRTimeSynchronizationClusterSetUTCTimeParams 

Class

# MTRTimeSynchronizationClusterSetUTCTimeParams

iOS 17.2+iPadOS 17.2+Mac Catalyst 17.2+macOS 14.2+tvOS 17.2+visionOS 1.0+watchOS 10.2+

``` source
class MTRTimeSynchronizationClusterSetUTCTimeParams
```

## Topics

### Instance Properties

var granularity: NSNumber

var serverSideProcessingTimeout: NSNumber?

Controls how much time, in seconds, we will allow for the server to process the command.

var timeSource: NSNumber?

var timedInvokeTimeoutMs: NSNumber?

Controls whether the command is a timed command (using Timed Invoke).

var utcTime: NSNumber

## Relationships

### Inherits From

- NSObject

### Inherited By

- MTRTimeSynchronizationClusterSetUtcTimeParams

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

