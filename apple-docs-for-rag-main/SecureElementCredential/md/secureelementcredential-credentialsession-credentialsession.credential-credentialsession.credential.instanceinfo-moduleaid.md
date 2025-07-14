

- SecureElementCredential
- CredentialSession
- CredentialSession.Credential
- CredentialSession.Credential.InstanceInfo
-  moduleAID 

Instance Property

# moduleAID

The module identifier of the package with which this instance is associated.

iOS 18.1+iPadOS 18.1+

``` source
let moduleAID: Data
```

## Discussion

The combination of the package identifier and this identifier indicates what type the associated applet instance is.

## See Also

### Inspecting instance identifiers

let instanceAID: Data

The unique identifier for the applet instance.

let packageAID: Data

The unique identifier of the package you use to install the instance.

