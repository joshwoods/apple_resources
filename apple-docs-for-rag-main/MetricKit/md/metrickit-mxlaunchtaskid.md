

- MetricKit
-  MXLaunchTaskID 

Structure

# MXLaunchTaskID

The task identifier to track launch measurements.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
struct MXLaunchTaskID
```

## Topics

### Creating a task identifier

init(String)

Creates a task identifer from a string.

init(rawValue: String)

Creates a task identifer from a string.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Measuring an extended launch

class func extendLaunchMeasurement(forTaskID: MXLaunchTaskID) throws

Starts to measure an extended launch task with the given task identifier.

class func finishExtendedLaunchMeasurement(forTaskID: MXLaunchTaskID) throws

Signals the end of an extended launch task.

