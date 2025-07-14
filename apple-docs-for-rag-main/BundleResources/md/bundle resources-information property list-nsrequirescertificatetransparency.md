

- Bundle Resources
- Information Property List
-  NSRequiresCertificateTransparency 

Property List Key

# NSRequiresCertificateTransparency

An obsolete Boolean value indicating whether to require Certificate Transparency.

iOS 9.0+iPadOS 9.0+macOS 10.11+visionOS 1.0+

## Details 

Type  

boolean

## Attributes 

Default: `NO`

## Discussion

Certificate Transparency (CT) is a protocol that ATS can use to identify mistakenly or maliciously issued X.509 certificates. Earlier versions of the system used this key to enable or disable CT for a given domain. Specifically, CT requires a domain’s server certificates to have support from signed CT timestamps from at least two CT logs trusted by Apple. For more information about Certificate Transparency, see RFC 6962.

The system now requires this behavior in all cases, making the key irrelevant.

Warning

Don’t use this key. The current system enforces this behavior, and new certificates can’t meet the requirement on older systems.

## See Also

### Exceptions

NSExceptionAllowsInsecureHTTPLoads

A Boolean value indicating whether to allow insecure HTTP loads.

NSExceptionMinimumTLSVersion

The minimum Transport Layer Security (TLS) version for network connections.

NSExceptionRequiresForwardSecrecy

A Boolean value indicating whether to override the perfect forward secrecy requirement.

