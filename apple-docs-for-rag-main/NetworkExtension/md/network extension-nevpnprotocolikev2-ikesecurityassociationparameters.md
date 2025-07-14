

- Network Extension
- NEVPNProtocolIKEv2
-  ikeSecurityAssociationParameters 

Instance Property

# ikeSecurityAssociationParameters

An NEVPNIKEv2SecurityAssociationParameters object containing the parameters for the initial IKE security association to be negotiated with the IKEv2 server.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
var ikeSecurityAssociationParameters: NEVPNIKEv2SecurityAssociationParameters { get }
```

## See Also

### Accessing IKEv2 Security Association parameters

var childSecurityAssociationParameters: NEVPNIKEv2SecurityAssociationParameters

An NEVPNIKEv2SecurityAssociationParameters object containing the parameters for the child IPSec security associations to be negotiated for each IKEv2 policy.

class NEVPNIKEv2SecurityAssociationParameters

Parameters for an IKEv2 Security Association.

