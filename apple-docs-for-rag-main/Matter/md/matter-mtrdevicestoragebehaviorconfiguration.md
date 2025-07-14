

- Matter
-  MTRDeviceStorageBehaviorConfiguration 

Class

# MTRDeviceStorageBehaviorConfiguration

Class that configures how MTRDevice objects persist their attributes to storage, so as to not overwhelm the underlying storage system.

iOS 17.6+iPadOS 17.6+Mac Catalyst 17.6+macOS 14.6+tvOS 17.6+visionOS 1.0+watchOS 10.6+

``` source
class MTRDeviceStorageBehaviorConfiguration
```

## Topics

### Initializers

convenience init(reportToPersistenceDelayTime: TimeInterval, reportToPersistenceDelayTimeMax: TimeInterval, recentReportTimesMaxCount: Int, timeBetweenReportsTooShortThreshold: TimeInterval, timeBetweenReportsTooShortMinThreshold: TimeInterval, reportToPersistenceDelayMaxMultiplier: Double, deviceReportingExcessivelyIntervalThreshold: TimeInterval)

Create configuration with specified values. See description below for details, and the list of properties below for valid ranges of these values.

### Instance Properties

var deviceReportingExcessivelyIntervalThreshold: TimeInterval

var disableStorageBehaviorOptimization: Bool

If disableStorageBehaviorOptimization is set to YES, then all the waiting mechanism as described above is disabled.

var recentReportTimesMaxCount: Int

var reportToPersistenceDelayMaxMultiplier: Double

var reportToPersistenceDelayTime: TimeInterval

If any of these properties are set to be out of the documented limits, these default values will be used to replace all of them:

var reportToPersistenceDelayTimeMax: TimeInterval

var timeBetweenReportsTooShortMinThreshold: TimeInterval

var timeBetweenReportsTooShortThreshold: TimeInterval

### Type Methods

class func withDefaultStorageBehavior() -> Self

Create configuration with a default set of values. See description below for details.

class func withStorageBehaviorOptimizationDisabled() -> Self

Create configuration that disables storage behavior optimizations.

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

