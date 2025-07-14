

- Authentication Services
- ASPasskeyAssertionCredential
-  init(userHandle:relyingParty:signature:clientDataHash:authenticatorData:credentialID:) 

Initializer

# init(userHandle:relyingParty:signature:clientDataHash:authenticatorData:credentialID:)

Initializes a passkey assertion credential object.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
init(
    userHandle: Data,
    relyingParty: String,
    signature: Data,
    clientDataHash: Data,
    authenticatorData: Data,
    credentialID: Data
)
```

## Parameters 

`userHandle`  

The user handle of this passkey.

`relyingParty`  

The relying party associated with this passkey.

`signature`  

The cryptographic signature of this credential.

`clientDataHash`  

A hash of the client data for this credential.

`authenticatorData`  

The authenticator data of the application that created this credential.

`credentialID`  

The identifier for this credential.

