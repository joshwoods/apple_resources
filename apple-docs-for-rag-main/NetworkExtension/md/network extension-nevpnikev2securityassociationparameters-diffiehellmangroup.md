

- Network Extension
- NEVPNIKEv2SecurityAssociationParameters
-  diffieHellmanGroup 

Instance Property

# diffieHellmanGroup

The Diffie Hellman group used by the Security Association.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
var diffieHellmanGroup: NEVPNIKEv2DiffieHellmanGroup { get set }
```

## Discussion

The default value of this property is NEVPNIKEv2DiffieHellmanGroup.group14.

The value of this property on childSecurityAssociationParameters of NEVPNProtocolIKEv2 only takes effect if the enablePFS of NEVPNProtocolIKEv2 is true (its default value is false).

## See Also

### IKEv2 Security Association parameters

var encryptionAlgorithm: NEVPNIKEv2EncryptionAlgorithm

The algorithm used by the Security Association to encrypt and decrypt data.

enum NEVPNIKEv2EncryptionAlgorithm

An enumeration of encryption algorithm values.

var integrityAlgorithm: NEVPNIKEv2IntegrityAlgorithm

The algorithm used by the Security Association to verify the integrity of data.

enum NEVPNIKEv2IntegrityAlgorithm

enum NEVPNIKEv2DiffieHellmanGroup

An enumeration of Diffie-Hellman group values.

var lifetimeMinutes: Int32

The duration of the lifetime of the Security Association, in minutes.

