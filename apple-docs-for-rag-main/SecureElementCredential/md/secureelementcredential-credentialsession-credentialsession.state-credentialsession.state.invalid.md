

- SecureElementCredential
- CredentialSession
- CredentialSession.State
-  CredentialSession.State.invalid 

Case

# CredentialSession.State.invalid

The state of an invalid credential session.

iOS 18.1+iPadOS 18.1+

``` source
case invalid
```

## Discussion

An invalid session is no longer available for use. To resume Secure Element credential functionality, call startSession() to create a new session.

## See Also

### Card session states

case management

The state for managing the credential session.

case wired(credential: CredentialSession.Credential)

The state for performing wired operations with a given credential.

case cardEmulation(credential: CredentialSession.Credential)

The state for performing card emulation with a given credential.

struct Credential

Information about a credential that a credential session retrieves from the Secure Element.

