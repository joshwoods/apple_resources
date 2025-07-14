

- Authentication Services
- ASPasskeyCredentialIdentity
-  init(relyingPartyIdentifier:userName:credentialID:userHandle:recordIdentifier:) 

Initializer

# init(relyingPartyIdentifier:userName:credentialID:userHandle:recordIdentifier:)

Creates and initializes a passkey credential identity.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
convenience init(
    relyingPartyIdentifier: String,
    userName: String,
    credentialID: Data,
    userHandle: Data,
    recordIdentifier: String?
)
```

## Return Value

The new credential identity object.

## See Also

### Creating a credential identity

convenience init(relyingPartyIdentifier: String, userName: String, credentialID: Data, userHandle: Data, recordIdentifier: String?)

Initializes a passkey credential identity.

