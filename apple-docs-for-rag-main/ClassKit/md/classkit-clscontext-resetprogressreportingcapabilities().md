

- ClassKit
- CLSContext
-  resetProgressReportingCapabilities() 

Instance Method

# resetProgressReportingCapabilities()

Resets the set of capabilities for the context.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
func resetProgressReportingCapabilities()
```

## Discussion

Use this method to remove all the capabilities that you previously added with the addProgressReportingCapabilities(_:) method. After calling the reset method, the context reverts to having only the default CLSProgressReportingCapability.Kind.duration capability that it had after initialization.

## See Also

### Indicating progress reporting capabilities

var progressReportingCapabilities: Set&lt;CLSProgressReportingCapability>

The kinds of progress reporting that the context can perform.

func addProgressReportingCapabilities(Set&lt;CLSProgressReportingCapability>)

Adds a progress reporting capability to the set of capabilities for the context.

class CLSProgressReportingCapability

A progress reporting capability supported by a context.

