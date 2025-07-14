

- SecureElementCredential
- CredentialSession
- CredentialSession.Credential
- CredentialSession.Credential.InstanceInfo
-  instanceAID 

Instance Property

# instanceAID

The unique identifier for the applet instance.

iOS 18.1+iPadOS 18.1+

``` source
let instanceAID: Data
```

## Discussion

Use this identifier in performWiredTransaction(using:over:instanceAID:) for UIKit or performTransactionInWiredMode(using:instanceAID:) for SwiftUI, and when selecting this instance to perform data transceiving.

## See Also

### Inspecting instance identifiers

let packageAID: Data

The unique identifier of the package you use to install the instance.

let moduleAID: Data

The module identifier of the package with which this instance is associated.

