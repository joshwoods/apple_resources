

- Security
-  SecAsn1AlgId Deprecated

Structure

# SecAsn1AlgId

A structure identifying an ASN.1 algorithm by its OID, and its corresponding parameters.

macOS 10.0–12.0Deprecated

``` source
struct SecAsn1AlgId
```

Deprecated

SecAsn1 is not supported

## Topics

### Algorithm Characteristics

var algorithm: SecAsn1Oid

var parameters: SecAsn1Item

### Creating a Structure

init()

init(algorithm: SecAsn1Oid, parameters: SecAsn1Item)

## Relationships

### Conforms To

- BitwiseCopyable

