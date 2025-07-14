

- Authentication Services
- ASPasskeyRegistrationCredential
-  init(relyingParty:clientDataHash:credentialID:attestationObject:) 

Initializer

# init(relyingParty:clientDataHash:credentialID:attestationObject:)

Initializes a passkey registration credential object.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
init(
    relyingParty: String,
    clientDataHash: Data,
    credentialID: Data,
    attestationObject: Data
)
```

## Parameters 

`relyingParty`  

The relying party associated with this passkey.

`clientDataHash`  

A hash of the client data for this credential.

`credentialID`  

The identifier for this credential.

`attestationObject`  

The attestation object for this passkey, which may contain an attestation statement and authenticator data.

