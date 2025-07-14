

- SecureElementCredential
- CredentialSession
- CredentialSession.Credential
- CredentialSession.Credential.State
-  CredentialSession.Credential.State.installationPending 

Case

# CredentialSession.Credential.State.installationPending

The credential installation is pending but isn’t complete.

iOS 18.1+iPadOS 18.1+

``` source
case installationPending
```

## Discussion

A credential is in this state after sending the provisioning request but before installation actually completes or fails.

## See Also

### Credential states

case installed(instances: [CredentialSession.Credential.InstanceInfo])

The credential installation is complete for one or more instances.

struct InstanceInfo

Information about an applet instance associated with a specific credential.

case installationFailed

The credential installation failed.

