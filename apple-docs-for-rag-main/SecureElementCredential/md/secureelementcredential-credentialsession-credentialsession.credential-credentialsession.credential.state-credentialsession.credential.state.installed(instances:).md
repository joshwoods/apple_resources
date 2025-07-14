

- SecureElementCredential
- CredentialSession
- CredentialSession.Credential
- CredentialSession.Credential.State
-  CredentialSession.Credential.State.installed(instances:) 

Case

# CredentialSession.Credential.State.installed(instances:)

The credential installation is complete for one or more instances.

iOS 18.1+iPadOS 18.1+

``` source
case installed(instances: [CredentialSession.Credential.InstanceInfo])
```

## Discussion

The associated value `instances` is an array of applet instances associated with the installed credential.

## See Also

### Credential states

case installationPending

The credential installation is pending but isn’t complete.

struct InstanceInfo

Information about an applet instance associated with a specific credential.

case installationFailed

The credential installation failed.

