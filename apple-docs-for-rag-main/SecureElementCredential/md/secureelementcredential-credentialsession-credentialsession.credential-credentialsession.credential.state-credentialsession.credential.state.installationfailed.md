

- SecureElementCredential
- CredentialSession
- CredentialSession.Credential
- CredentialSession.Credential.State
-  CredentialSession.Credential.State.installationFailed 

Case

# CredentialSession.Credential.State.installationFailed

The credential installation failed.

iOS 18.1+iPadOS 18.1+

``` source
case installationFailed
```

## Discussion

A credential is only in this state following a failed installation. Prior to success or failure, the state is CredentialSession.Credential.State.installationPending.

## See Also

### Credential states

case installationPending

The credential installation is pending but isn’t complete.

case installed(instances: [CredentialSession.Credential.InstanceInfo])

The credential installation is complete for one or more instances.

struct InstanceInfo

Information about an applet instance associated with a specific credential.

