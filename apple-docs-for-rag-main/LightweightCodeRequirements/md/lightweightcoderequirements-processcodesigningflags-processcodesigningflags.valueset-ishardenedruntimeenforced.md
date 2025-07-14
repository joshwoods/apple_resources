

- LightweightCodeRequirements
- ProcessCodeSigningFlags
- ProcessCodeSigningFlags.ValueSet
-  isHardenedRuntimeEnforced 

Type Property

# isHardenedRuntimeEnforced

Flag indicating that the process has enabled the Hardened Runtime

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.1+watchOS 10.4+

``` source
static let isHardenedRuntimeEnforced: ProcessCodeSigningFlags.ValueSet
```

## Discussion

This flag may be present on any on disk signature. This flag only has effect on main executables. This flag only has effect on macOS. On iOS/watchOS/tvOS/visionOS most of the same policies are enforced regardless of the state of this flag. This is equivalent to `CS_RUNTIME` in C APIs.

