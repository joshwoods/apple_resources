

- Authentication Services
- ASPasskeyCredentialIdentity
-  init(relyingPartyIdentifier:userName:credentialID:userHandle:recordIdentifier:) 

Initializer

# init(relyingPartyIdentifier:userName:credentialID:userHandle:recordIdentifier:)

Initializes a passkey credential identity.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
convenience init(
    relyingPartyIdentifier: String,
    userName: String,
    credentialID: Data,
    userHandle: Data,
    recordIdentifier: String? = nil
)
```

## Parameters 

`relyingPartyIdentifier`  

The relying party identifier associated with this credential.

`userName`  

The username associated with this credential.

`credentialID`  

The credential identifier for this credential.

`userHandle`  

The user handle associated with this credential.

`recordIdentifier`  

The record identifier for this credential.

## See Also

### Creating a credential identity

convenience init(relyingPartyIdentifier: String, userName: String, credentialID: Data, userHandle: Data, recordIdentifier: String?)

Creates and initializes a passkey credential identity.

