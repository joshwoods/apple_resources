

- Network Extension
-  NEVPNIKEv2SecurityAssociationParameters 

Class

# NEVPNIKEv2SecurityAssociationParameters

Parameters for an IKEv2 Security Association.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
class NEVPNIKEv2SecurityAssociationParameters
```

## Topics

### IKEv2 Security Association parameters

var encryptionAlgorithm: NEVPNIKEv2EncryptionAlgorithm

The algorithm used by the Security Association to encrypt and decrypt data.

enum NEVPNIKEv2EncryptionAlgorithm

An enumeration of encryption algorithm values.

var integrityAlgorithm: NEVPNIKEv2IntegrityAlgorithm

The algorithm used by the Security Association to verify the integrity of data.

enum NEVPNIKEv2IntegrityAlgorithm

var diffieHellmanGroup: NEVPNIKEv2DiffieHellmanGroup

The Diffie Hellman group used by the Security Association.

enum NEVPNIKEv2DiffieHellmanGroup

An enumeration of Diffie-Hellman group values.

var lifetimeMinutes: Int32

The duration of the lifetime of the Security Association, in minutes.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Accessing IKEv2 Security Association parameters

var ikeSecurityAssociationParameters: NEVPNIKEv2SecurityAssociationParameters

An NEVPNIKEv2SecurityAssociationParameters object containing the parameters for the initial IKE security association to be negotiated with the IKEv2 server.

var childSecurityAssociationParameters: NEVPNIKEv2SecurityAssociationParameters

An NEVPNIKEv2SecurityAssociationParameters object containing the parameters for the child IPSec security associations to be negotiated for each IKEv2 policy.

