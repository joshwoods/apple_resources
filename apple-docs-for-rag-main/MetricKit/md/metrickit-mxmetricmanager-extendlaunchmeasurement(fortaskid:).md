

- MetricKit
- MXMetricManager
-  extendLaunchMeasurement(forTaskID:) 

Type Method

# extendLaunchMeasurement(forTaskID:)

Starts to measure an extended launch task with the given task identifier.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
class func extendLaunchMeasurement(forTaskID taskID: MXLaunchTaskID) throws
```

## Parameters 

`taskID`  

The task identifier. Must be a unique, `non-null` string.

## Discussion

Use this method on the main thread to measure an extended launch task. Your app needs to start the first task before or during scene(_:restoreInteractionStateWith:), or before the system calls sceneDidBecomeActive(_:) on the first scene to connect, and each task needs to overlap with others.

The maximum number of tasks is 16. The extended launch measurement finishes when all running tasks finish.

## See Also

### Measuring an extended launch

class func finishExtendedLaunchMeasurement(forTaskID: MXLaunchTaskID) throws

Signals the end of an extended launch task.

struct MXLaunchTaskID

The task identifier to track launch measurements.

