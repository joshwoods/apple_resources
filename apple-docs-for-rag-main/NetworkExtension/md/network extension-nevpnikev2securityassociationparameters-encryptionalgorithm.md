

- Network Extension
- NEVPNIKEv2SecurityAssociationParameters
-  encryptionAlgorithm 

Instance Property

# encryptionAlgorithm

The algorithm used by the Security Association to encrypt and decrypt data.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
var encryptionAlgorithm: NEVPNIKEv2EncryptionAlgorithm { get set }
```

## Discussion

The default value of this property is NEVPNIKEv2EncryptionAlgorithm.algorithmAES256, except on tvOS where the default is NEVPNIKEv2EncryptionAlgorithm.algorithmAES256GCM.

## See Also

### IKEv2 Security Association parameters

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

