

- MetricKit
- MXMetricManager
-  finishExtendedLaunchMeasurement(forTaskID:) 

Type Method

# finishExtendedLaunchMeasurement(forTaskID:)

Signals the end of an extended launch task.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
class func finishExtendedLaunchMeasurement(forTaskID taskID: MXLaunchTaskID) throws
```

## Parameters 

`taskID`  

The task identifier. Must be a unique, `non-null` string.

## Discussion

Use this method on the main thread to end an extended launch task previously started with extendLaunchMeasurement(forTaskID:).

## See Also

### Measuring an extended launch

class func extendLaunchMeasurement(forTaskID: MXLaunchTaskID) throws

Starts to measure an extended launch task with the given task identifier.

struct MXLaunchTaskID

The task identifier to track launch measurements.

