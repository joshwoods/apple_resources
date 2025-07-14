

- MetricKit
-  mxSignpostAnimationIntervalBegin(dso:log:name:signpostID:\_:\_:) 

Function

# mxSignpostAnimationIntervalBegin(dso:log:name:signpostID:\_:\_:)

Posts the start time of an animation interval to the log system.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
func mxSignpostAnimationIntervalBegin(
    dso: UnsafeRawPointer = #dsohandle,
    log: OSLog,
    name: StaticString,
    signpostID: OSSignpostID = .exclusive,
    _ format: StaticString = "isAnimation=YES \n%{public, signpost:metrics}@",
    _ arguments: [any CVarArg] = [Unmanaged.fromOpaque(_MXSignpostMetricsSnapshot()).takeUnretainedValue()]
)
```

## Parameters 

`dso`  

A parameter for internal system use.

`log`  

A log object to log the signpost to.

`name`  

A string containing the developer-assigned name of the custom event.

`signpostID`  

A parameter for internal system use.

`format`  

A parameter for internal system use.

`arguments`  

An array of arguments with a format string, followed by the expected number of arguments in the order that they appear in the string.

## Discussion

Call this function to mark the beginning of an animation interval in the metric kit log. Provide a `log` that you create with makeLogHandle(category:), a `name` for the event, and variable `arguments` for os_signpost_event_emit. Don’t alter the parameters `dso`, `signpostID`, or `format`.

## See Also

### Logging custom metrics

func mxSignpost(OSSignpostType, dso: UnsafeRawPointer, log: OSLog, name: StaticString, signpostID: OSSignpostID, StaticString, [any CVarArg])

Posts a single custom metric, the start time of a custom metric, or the end time of a custom metric to the log system.

