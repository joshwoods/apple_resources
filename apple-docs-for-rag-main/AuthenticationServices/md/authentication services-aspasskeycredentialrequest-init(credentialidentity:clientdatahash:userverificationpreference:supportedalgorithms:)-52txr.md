

- Authentication Services
- ASPasskeyCredentialRequest
-  init(credentialIdentity:clientDataHash:userVerificationPreference:supportedAlgorithms:) 

Initializer

# init(credentialIdentity:clientDataHash:userVerificationPreference:supportedAlgorithms:)

Initializes a passkey credential request.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
convenience init(
    credentialIdentity: ASPasskeyCredentialIdentity,
    clientDataHash: Data,
    userVerificationPreference: ASAuthorizationPublicKeyCredentialUserVerificationPreference,
    supportedAlgorithms: [ASCOSEAlgorithmIdentifier]
)
```

## Parameters 

`credentialIdentity`  

The identity of the requested passkey credential.

`clientDataHash`  

Hash of the client data from the passkey authentication challenge.

`userVerificationPreference`  

The relying party’s user verification preference.

`supportedAlgorithms`  

A list of cryptographic signature algorithms that the relying party supports.

## Discussion

For credential assertion requests, supply an empty array for the `supportedAlgorithms`. For credential registration requests, supply an array of one or more ASCOSEAlgorithmIdentifier values.

## See Also

### Creating passkey credential requests

convenience init(credentialIdentity: ASPasskeyCredentialIdentity, clientDataHash: Data, userVerificationPreference: ASAuthorizationPublicKeyCredentialUserVerificationPreference, supportedAlgorithms: [NSNumber])

Initializes a passkey credential request.

