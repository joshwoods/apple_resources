

- Matter
- MTRDeviceStorageBehaviorConfiguration
-  init(reportToPersistenceDelayTime:reportToPersistenceDelayTimeMax:recentReportTimesMaxCount:timeBetweenReportsTooShortThreshold:timeBetweenReportsTooShortMinThreshold:reportToPersistenceDelayMaxMultiplier:deviceReportingExcessivelyIntervalThreshold:) 

Initializer

# init(reportToPersistenceDelayTime:reportToPersistenceDelayTimeMax:recentReportTimesMaxCount:timeBetweenReportsTooShortThreshold:timeBetweenReportsTooShortMinThreshold:reportToPersistenceDelayMaxMultiplier:deviceReportingExcessivelyIntervalThreshold:)

Create configuration with specified values. See description below for details, and the list of properties below for valid ranges of these values.

iOS 17.6+iPadOS 17.6+Mac Catalyst 17.6+macOS 14.6+tvOS 17.6+visionOS 1.0+watchOS 10.6+

``` source
convenience init(
    reportToPersistenceDelayTime: TimeInterval,
    reportToPersistenceDelayTimeMax: TimeInterval,
    recentReportTimesMaxCount: Int,
    timeBetweenReportsTooShortThreshold: TimeInterval,
    timeBetweenReportsTooShortMinThreshold: TimeInterval,
    reportToPersistenceDelayMaxMultiplier: Double,
    deviceReportingExcessivelyIntervalThreshold: TimeInterval
)
```

