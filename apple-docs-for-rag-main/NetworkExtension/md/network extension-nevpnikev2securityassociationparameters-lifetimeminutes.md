

- Network Extension
- NEVPNIKEv2SecurityAssociationParameters
-  lifetimeMinutes 

Instance Property

# lifetimeMinutes

The duration of the lifetime of the Security Association, in minutes.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
var lifetimeMinutes: Int32 { get set }
```

## Discussion

The default is 60 for IKE Security Associations, and 30 for Child Security Associations. Before the end of the lifetime is reached, IKEv2 will attempt to negotiate new keys for the Security Association in order to maintain the IKEv2 session.

## See Also

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

