

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
    supportedAlgorithms: [NSNumber]
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

An array of numbers that represent cryptographic signature algorithms the identifying party supports.

## Discussion

The `supportedAlgorithms` parameter is empty for credential assertion requests. For credential registration requests, it contains one or more numbers from the Internet Assigned Numbers Authority (IANA) Concise Binary Object Representation Object Signing and Encryption (COSE) algorithms registry.

## See Also

### Creating passkey credential requests

convenience init(credentialIdentity: ASPasskeyCredentialIdentity, clientDataHash: Data, userVerificationPreference: ASAuthorizationPublicKeyCredentialUserVerificationPreference, supportedAlgorithms: [ASCOSEAlgorithmIdentifier])

Initializes a passkey credential request.

