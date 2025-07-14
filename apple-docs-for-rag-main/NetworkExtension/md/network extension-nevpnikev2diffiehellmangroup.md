

- Network Extension
-  NEVPNIKEv2DiffieHellmanGroup 

Enumeration

# NEVPNIKEv2DiffieHellmanGroup

An enumeration of Diffie-Hellman group values.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
enum NEVPNIKEv2DiffieHellmanGroup
```

## Topics

### Diffie-Hellman groups

case groupInvalid

A value indicating the group is not a valid Diffie-Hellman group.

case group1

Diffie Hellman group 1 (768-bit modular exponential \[MODP\]).

Deprecated

case group2

Diffie Hellman group 2 (1024-bit modular exponential \[MODP\]).

Deprecated

case group5

Diffie Hellman group 5 (1536-bit modular exponential \[MODP\]).

Deprecated

case group14

Diffie Hellman group 14 (2048-bit modular exponential \[MODP\]).

case group15

Diffie Hellman group 15 (3072-bit modular exponential \[MODP\]).

case group16

Diffie Hellman group 16 (4096-bit modular exponential \[MODP\]).

case group17

Diffie Hellman group 17 (6144-bit modular exponential \[MODP\]).

case group18

Diffie Hellman group 18 (8192-bit modular exponential \[MODP\]).

case group19

Diffie Hellman group 19 (256-bit random elliptic curve group over GF\[P\] \[ECP\]).

case group20

Diffie Hellman group 20 (384-bit random elliptic curve group over GF\[P\] \[ECP\]).

case group21

Diffie Hellman group 21 (521-bit random elliptic curve group over GF\[P\] \[ECP\]).

case group31

Diffie Hellman group 31 (Curve 25519).

case group32

Diffie Hellman group 32 (Curve 448).

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

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

var lifetimeMinutes: Int32

The duration of the lifetime of the Security Association, in minutes.

