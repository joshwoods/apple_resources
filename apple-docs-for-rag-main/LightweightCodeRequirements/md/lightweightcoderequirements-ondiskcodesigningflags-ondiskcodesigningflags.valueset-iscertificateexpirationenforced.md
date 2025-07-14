

- LightweightCodeRequirements
- OnDiskCodeSigningFlags
- OnDiskCodeSigningFlags.ValueSet
-  isCertificateExpirationEnforced 

Type Property

# isCertificateExpirationEnforced

Flag indicating that the signature on this code should be treated as invalid if the certificate it was signed with expired.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.1+watchOS 10.4+

``` source
static let isCertificateExpirationEnforced: OnDiskCodeSigningFlags.ValueSet
```

## Discussion

By default code signatures are valid if the certificate they were signed with was valid at the time of signing. This flag invalidates signatures from certificatest that are expired at the time of use. This is equivalent to `CS_CHECK_EXPIRATION` in C APIs.

