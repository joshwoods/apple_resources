

- LightweightCodeRequirements
- ProcessCodeSigningFlags
- ProcessCodeSigningFlags.ValueSet
-  isDebugged 

Type Property

# isDebugged

Flag indicating that the process has been attached by a debugger.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.1+watchOS 10.4+

``` source
static let isDebugged: ProcessCodeSigningFlags.ValueSet
```

## Discussion

This is equivalent to `CS_DEBUGGED` in C APIs.

