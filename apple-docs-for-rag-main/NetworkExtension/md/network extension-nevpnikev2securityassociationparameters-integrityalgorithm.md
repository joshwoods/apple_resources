

- Network Extension
- NEVPNIKEv2SecurityAssociationParameters
-  integrityAlgorithm 

Instance Property

# integrityAlgorithm

The algorithm used by the Security Association to verify the integrity of data.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
var integrityAlgorithm: NEVPNIKEv2IntegrityAlgorithm { get set }
```

## Discussion

The default value of this property is NEVPNIKEv2IntegrityAlgorithm.SHA256.

The system infers its IKE psedo-random number generation algorithm based on the integrity algorithm.

## See Also

### IKEv2 Security Association parameters

var encryptionAlgorithm: NEVPNIKEv2EncryptionAlgorithm

The algorithm used by the Security Association to encrypt and decrypt data.

enum NEVPNIKEv2EncryptionAlgorithm

An enumeration of encryption algorithm values.

enum NEVPNIKEv2IntegrityAlgorithm

var diffieHellmanGroup: NEVPNIKEv2DiffieHellmanGroup

The Diffie Hellman group used by the Security Association.

enum NEVPNIKEv2DiffieHellmanGroup

An enumeration of Diffie-Hellman group values.

var lifetimeMinutes: Int32

The duration of the lifetime of the Security Association, in minutes.

