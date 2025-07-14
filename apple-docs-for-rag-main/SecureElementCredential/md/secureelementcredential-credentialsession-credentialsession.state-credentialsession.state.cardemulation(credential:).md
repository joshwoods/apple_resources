

- SecureElementCredential
- CredentialSession
- CredentialSession.State
-  CredentialSession.State.cardEmulation(credential:) 

Case

# CredentialSession.State.cardEmulation(credential:)

The state for performing card emulation with a given credential.

iOS 18.1+iPadOS 18.1+

``` source
case cardEmulation(credential: CredentialSession.Credential)
```

## Parameters 

`credential`  

The credential currently in use by the session.

## Mentioned in 

Accessing and using secure element credentials

## Discussion

In the card emulation state, the session makes the selected credential available to NFC contactless readers.

## See Also

### Card session states

case management

The state for managing the credential session.

case wired(credential: CredentialSession.Credential)

The state for performing wired operations with a given credential.

struct Credential

Information about a credential that a credential session retrieves from the Secure Element.

case invalid

The state of an invalid credential session.

