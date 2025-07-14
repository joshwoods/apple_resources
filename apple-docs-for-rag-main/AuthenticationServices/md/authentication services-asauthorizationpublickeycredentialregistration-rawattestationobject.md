

- Authentication Services
- ASAuthorizationPublicKeyCredentialRegistration
-  rawAttestationObject 

Instance Property

# rawAttestationObject

A data object that contains the returned attestation.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
var rawAttestationObject: Data? { get }
```

**Required**

## Discussion

This object contains the public key. If you request it, it also contains the attestation statement. To learn more, see the W3C Web Authentication specification.

