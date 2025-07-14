

- ClassKit
- CLSProgressReportingCapability
-  init(kind:details:) 

Initializer

# init(kind:details:)

Creates a new progress reporting capability of the given type with a descriptive string.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
init(
    kind: CLSProgressReportingCapability.Kind,
    details: String?
)
```

## Parameters 

`kind`  

The type of progress reporting, like duration or a final score, that this capability represents.

`details`  

A description of the metric, given as a localized string.

