

- SecureElementCredential
- CredentialSession
- CredentialSession.State
-  CredentialSession.State.management 

Case

# CredentialSession.State.management

The state for managing the credential session.

iOS 18.1+iPadOS 18.1+

``` source
case management
```

## Mentioned in 

Accessing and using secure element credentials

## Discussion

In this state, the session can list all credentials and can add and delete individual credentials.

## See Also

### Card session states

case wired(credential: CredentialSession.Credential)

The state for performing wired operations with a given credential.

case cardEmulation(credential: CredentialSession.Credential)

The state for performing card emulation with a given credential.

struct Credential

Information about a credential that a credential session retrieves from the Secure Element.

case invalid

The state of an invalid credential session.

