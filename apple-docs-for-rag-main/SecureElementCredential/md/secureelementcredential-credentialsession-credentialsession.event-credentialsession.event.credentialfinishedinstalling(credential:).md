

- SecureElementCredential
- CredentialSession
- CredentialSession.Event
-  CredentialSession.Event.credentialFinishedInstalling(credential:) 

Case

# CredentialSession.Event.credentialFinishedInstalling(credential:)

The session finished installing a credential.

iOS 18.1+iPadOS 18.1+

``` source
case credentialFinishedInstalling(credential: CredentialSession.Credential)
```

## Discussion

The associated value `credential` indicates which credential finished installing.

Note

The session doesn’t send this event if a credential fails to install. Instead, the credential remains in the CredentialSession.Credential.State.installationPending state until the app calls listCredentials(). This call allows the framework to confirm that the installation failed and transitions the credential state to CredentialSession.Credential.State.installationFailed.

## See Also

### Credential events

struct Credential

Information about a credential that a credential session retrieves from the Secure Element.

