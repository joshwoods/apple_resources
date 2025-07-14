

- Security
-  SecAsn1PubKeyInfo Deprecated

Structure

# SecAsn1PubKeyInfo

A structure containing a public key and its associated algorithm.

macOS 10.0–12.0Deprecated

``` source
struct SecAsn1PubKeyInfo
```

Deprecated

SecAsn1 is not supported

## Topics

### Public Key Characteristics

var subjectPublicKey: SecAsn1Item

var algorithm: SecAsn1AlgId

### Creating a Public Key

init()

init(algorithm: SecAsn1AlgId, subjectPublicKey: SecAsn1Item)

## Relationships

### Conforms To

- BitwiseCopyable

