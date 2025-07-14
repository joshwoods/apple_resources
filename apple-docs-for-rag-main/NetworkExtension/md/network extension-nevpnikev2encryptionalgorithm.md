

- Network Extension
-  NEVPNIKEv2EncryptionAlgorithm 

Enumeration

# NEVPNIKEv2EncryptionAlgorithm

An enumeration of encryption algorithm values.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
enum NEVPNIKEv2EncryptionAlgorithm
```

## Topics

### Encryption algorithms

case algorithmDES

Data Encryption Standard (DES)

Deprecated

case algorithm3DES

Triple Data Encryption Algorithm (aka 3DES)

Deprecated

case algorithmAES128

Advanced Encryption Standard 256-bit (AES256).

Deprecated

case algorithmAES256

Advanced Encryption Standard 256 bit (AES256).

case algorithmAES128GCM

Advanced Encryption Standard 128-bit Galois/Counter Mode (AES128GCM).

Deprecated

case algorithmAES256GCM

Advanced Encryption Standard 256-bit Galois/Counter Mode (AES256GCM).

case algorithmChaCha20Poly1305

ChaCha20 and Poly1305 (ChaCha20Poly1305).

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

var integrityAlgorithm: NEVPNIKEv2IntegrityAlgorithm

The algorithm used by the Security Association to verify the integrity of data.

enum NEVPNIKEv2IntegrityAlgorithm

var diffieHellmanGroup: NEVPNIKEv2DiffieHellmanGroup

The Diffie Hellman group used by the Security Association.

enum NEVPNIKEv2DiffieHellmanGroup

An enumeration of Diffie-Hellman group values.

var lifetimeMinutes: Int32

The duration of the lifetime of the Security Association, in minutes.

