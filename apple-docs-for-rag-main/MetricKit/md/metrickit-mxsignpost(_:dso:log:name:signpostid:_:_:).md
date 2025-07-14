

- MetricKit
-  mxSignpost(\_:dso:log:name:signpostID:\_:\_:) 

Function

# mxSignpost(\_:dso:log:name:signpostID:\_:\_:)

Posts a single custom metric, the start time of a custom metric, or the end time of a custom metric to the log system.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+visionOS 1.0+

``` source
func mxSignpost(
    _ type: OSSignpostType,
    dso: UnsafeRawPointer = #dsohandle,
    log: OSLog,
    name: StaticString,
    signpostID: OSSignpostID = .exclusive,
    _ format: StaticString = "%{public, signpost:metrics}@",
    _ arguments: [any CVarArg] = [Unmanaged.fromOpaque(_MXSignpostMetricsSnapshot()).takeUnretainedValue()]
)
```

## Parameters 

`type`  

A value that represents the type of the signpost:

- `event`: A single custom metric.

- `begin`: The start time of a custom metric.

- `end`: The end time of a custom metric.

`dso`  

A parameter for internal system use.

`log`  

A log for the category of the event that was created previously using makeLogHandle(category:).

`name`  

A string containing the developer-assigned name of the custom event.

`signpostID`  

A parameter for internal system use.

`format`  

A parameter for internal system use.

`arguments`  

The variable arguments for os_signpost_event_emit.

## Discussion

Call this function to mark a custom metric, custom metric start time, or custom metric end time in the metric kit log. Provide a `log` that you create with makeLogHandle(category:), the `type` of the event, a `name` for the event, and variable `arguments` for os_signpost_event_emit. Don’t alter the parameters `dso`, `signpostID`, or `format`.

## See Also

### Logging custom metrics

func mxSignpostAnimationIntervalBegin(dso: UnsafeRawPointer, log: OSLog, name: StaticString, signpostID: OSSignpostID, StaticString, [any CVarArg])

Posts the start time of an animation interval to the log system.

