

- ClassKit
- CLSContext
-  addProgressReportingCapabilities(\_:) 

Instance Method

# addProgressReportingCapabilities(\_:)

Adds a progress reporting capability to the set of capabilities for the context.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
func addProgressReportingCapabilities(_ capabilities: Set)
```

## Discussion

Use this method at the time you create a context to indicate what kinds of metrics, like duration, a score, or a binary result, that you record for the context. This helps teachers to understand what to expect when assigning a context.

By default, all contexts have a CLSProgressReportingCapability.Kind.duration capability, because the framework records duration automatically. But you can add others, according to which metrics you record. You can also add another duration capability, but because a context can have only one capability of a given kind, yours supersedes the default.

To remove all capabilities that you previously added, call the resetProgressReportingCapabilities() method. This restores the context to its default state, which is to have only the default duration capability.

## See Also

### Indicating progress reporting capabilities

var progressReportingCapabilities: Set&lt;CLSProgressReportingCapability>

The kinds of progress reporting that the context can perform.

func resetProgressReportingCapabilities()

Resets the set of capabilities for the context.

class CLSProgressReportingCapability

A progress reporting capability supported by a context.

