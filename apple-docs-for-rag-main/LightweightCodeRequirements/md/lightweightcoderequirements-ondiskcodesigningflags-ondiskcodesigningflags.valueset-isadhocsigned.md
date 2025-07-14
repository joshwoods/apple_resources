

- LightweightCodeRequirements
- OnDiskCodeSigningFlags
- OnDiskCodeSigningFlags.ValueSet
-  isAdhocSigned 

Type Property

# isAdhocSigned

The code is adhoc signed i.e. it contains a code directory and page hashes but no CMS signature.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.1+watchOS 10.4+

``` source
static let isAdhocSigned: OnDiskCodeSigningFlags.ValueSet
```

## Discussion

This is equivalent to `CS_ADHOC` in C APIs.

