

- Bundle Resources
- Information Property List
-  NSExceptionAllowsInsecureHTTPLoads 

Property List Key

# NSExceptionAllowsInsecureHTTPLoads

A Boolean value indicating whether to allow insecure HTTP loads.

iOS 9.0+iPadOS 9.0+macOS 10.11+visionOS 1.0+

## Details 

Type  

boolean

## Attributes 

Default: `NO`

## Discussion

Set the value for this key to `YES` to allow insecure HTTP loads for the given domain, or to be able to loosen the server trust evaluation requirements for HTTPS connections to the domain, as described in Performing manual server trust authentication.

Using this key doesn’t by itself change default server trust evaluation requirements for HTTPS connections, described in `Ensure the Network Server Meets Minimum Requirements`. Using only this key also doesn’t change the TLS or forward secrecy requirements imposed by ATS. As a result, you might need to combine this key with the NSExceptionMinimumTLSVersion or NSExceptionRequiresForwardSecrecy key in certain cases.

This key is optional. The default value is `NO`.

Important

You must supply a justification during App Store review if you set the key’s value to YES, as described in `Provide Justification for Exceptions`.

## See Also

### Exceptions

NSExceptionMinimumTLSVersion

The minimum Transport Layer Security (TLS) version for network connections.

NSExceptionRequiresForwardSecrecy

A Boolean value indicating whether to override the perfect forward secrecy requirement.

NSRequiresCertificateTransparency

An obsolete Boolean value indicating whether to require Certificate Transparency.

