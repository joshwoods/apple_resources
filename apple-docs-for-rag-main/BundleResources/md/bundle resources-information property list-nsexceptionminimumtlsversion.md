

- Bundle Resources
- Information Property List
-  NSExceptionMinimumTLSVersion 

Property List Key

# NSExceptionMinimumTLSVersion

The minimum Transport Layer Security (TLS) version for network connections.

iOS 9.0+iPadOS 9.0+macOS 10.11+visionOS 1.0+

## Details 

Type  

string

## Possible Values 

`TLSv1.0`  

Require a minimum TLS version of 1.0.

`TLSv1.1`  

Require a minimum TLS version of 1.1.

`TLSv1.2`  

Require a minimum TLS version of 1.2.

`TLSv1.3`  

Require a minimum TLS version of 1.3.

## Attributes 

Default: `TLSv1.2`

## Discussion

This key is optional. The value is a string, with a default value of `TLSv1.2`.

Important

You must supply a justification during App Store review if you use this key to set a protocol version lower than 1.2, as described in `Provide Justification for Exceptions`.

## See Also

### Exceptions

NSExceptionAllowsInsecureHTTPLoads

A Boolean value indicating whether to allow insecure HTTP loads.

NSExceptionRequiresForwardSecrecy

A Boolean value indicating whether to override the perfect forward secrecy requirement.

NSRequiresCertificateTransparency

An obsolete Boolean value indicating whether to require Certificate Transparency.

