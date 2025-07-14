

- LightweightCodeRequirements
- ProcessCodeSigningFlags
- ProcessCodeSigningFlags.ValueSet
-  isSignedByLinker 

Type Property

# isSignedByLinker

Flag indicating that the code was signed by the linker and not an invocation of codesign.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.1+watchOS 10.4+

``` source
static let isSignedByLinker: ProcessCodeSigningFlags.ValueSet
```

## Discussion

This is equivalent to `CS_LINKER_SIGNED` in C APIs.

