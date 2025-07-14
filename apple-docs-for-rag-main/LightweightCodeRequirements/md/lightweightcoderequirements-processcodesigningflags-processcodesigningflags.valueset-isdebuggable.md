

- LightweightCodeRequirements
- ProcessCodeSigningFlags
- ProcessCodeSigningFlags.ValueSet
-  isDebuggable 

Type Property

# isDebuggable

Flag indicating that the process is debuggable by authorized debuggers.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.1+watchOS 10.4+

``` source
static let isDebuggable: ProcessCodeSigningFlags.ValueSet
```

## Discussion

This is equivalent to `CS_GET_TASK_ALLOW` in C APIs.

