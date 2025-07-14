

- LightweightCodeRequirements
- ProcessCodeSigningFlags
- ProcessCodeSigningFlags.ValueSet
-  isLibraryValidationRequired 

Type Property

# isLibraryValidationRequired

Flag indicating that the process should enforce Library Validation.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.1+watchOS 10.4+

``` source
static let isLibraryValidationRequired: ProcessCodeSigningFlags.ValueSet
```

## Discussion

Library validation means that the process will only load Apple signed code and code signed by the same Team Identifier as the process. This flag may be present on any on disk signature. This flag only has effect on main executables. This flag only has effect on macOS processes. On iOS/watchOS/tvOS/visionOS and iOS apps on macOS all processes enforce Library Validation, regardless of the state of this flag. This is equivalent to `CS_REQUIRE_LV` in C APIs.

