

- Security
-  SecExternalItemType 

Enumeration

# SecExternalItemType

The import item type.

macOS 10.0+

``` source
enum SecExternalItemType
```

## Topics

### Constants

case itemTypeUnknown

Indicates that the caller does not know the type of information being imported or exported.

case itemTypePrivateKey

Indicates a private key.

case itemTypePublicKey

Indicates a public key.

case itemTypeSessionKey

Indicates a session key.

case itemTypeCertificate

Indicates a certificate.

case itemTypeAggregate

Indicates a set of certificates or certificates and private keys.

### Initializers

init?(rawValue: UInt32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

