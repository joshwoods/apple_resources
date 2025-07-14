

- Authentication Services
- ASImportableCredential
- ASImportableCredential.Passkey
-  init(credentialID:relyingPartyIdentifier:userName:userDisplayName:userHandle:key:) 

Initializer

# init(credentialID:relyingPartyIdentifier:userName:userDisplayName:userHandle:key:)

Creates a passkey instance.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+visionOS 2.2+

``` source
init(
    credentialID: Data,
    relyingPartyIdentifier: String,
    userName: String,
    userDisplayName: String,
    userHandle: Data,
    key: Data
)
```

## Parameters 

`credentialID`  

The credential ID associated with this passkey.

`relyingPartyIdentifier`  

The relying party identifier associated with the passkey

`userName`  

The username associated with the passkey.

`userDisplayName`  

The human-readable name associated with the passkey.

`userHandle`  

The user handle associated with the passkey.

`key`  

The private key associated with this passkey.

