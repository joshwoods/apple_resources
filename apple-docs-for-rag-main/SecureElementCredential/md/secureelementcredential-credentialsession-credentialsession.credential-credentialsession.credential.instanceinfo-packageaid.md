

- SecureElementCredential
- CredentialSession
- CredentialSession.Credential
- CredentialSession.Credential.InstanceInfo
-  packageAID 

Instance Property

# packageAID

The unique identifier of the package you use to install the instance.

iOS 18.1+iPadOS 18.1+

``` source
let packageAID: Data
```

## Discussion

You can use the version encoded in this identifier to determine the version of the installed applet.

## See Also

### Inspecting instance identifiers

let instanceAID: Data

The unique identifier for the applet instance.

let moduleAID: Data

The module identifier of the package with which this instance is associated.

