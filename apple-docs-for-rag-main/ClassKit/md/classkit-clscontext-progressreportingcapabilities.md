

- ClassKit
- CLSContext
-  progressReportingCapabilities 

Instance Property

# progressReportingCapabilities

The kinds of progress reporting that the context can perform.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
var progressReportingCapabilities: Set { get }
```

## Discussion

Use progress reporting capabilities to tell teachers what kinds of metrics — like duration, percentage completion, or a score — that a context records.

By default, all contexts have a CLSProgressReportingCapability.Kind.duration capability, because the framework automatically measures time spent on activities — the time between when you call the start() and stop() methods. You can add one or more other capabilities using the addProgressReportingCapabilities(_:) method, corresponding to the other kinds of activity that you report for a context. For example, if you set the progress property of an activity, add the CLSProgressReportingCapability.Kind.percent capability. Typically, you perform this configuration when creating the context.

The values that you put in the progress reporting capability set don’t affect your ability to record metrics. But they do affect the presentation of your app in the Schoolwork app.

To revert to the default state of reporting only duration, call the resetProgressReportingCapabilities() method.

## See Also

### Indicating progress reporting capabilities

func addProgressReportingCapabilities(Set&lt;CLSProgressReportingCapability>)

Adds a progress reporting capability to the set of capabilities for the context.

func resetProgressReportingCapabilities()

Resets the set of capabilities for the context.

class CLSProgressReportingCapability

A progress reporting capability supported by a context.

