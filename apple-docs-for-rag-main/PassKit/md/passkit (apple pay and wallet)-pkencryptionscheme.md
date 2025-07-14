

- PassKit (Apple Pay and Wallet)
-  PKEncryptionScheme 

Structure

# PKEncryptionScheme

Encryption schemes.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
struct PKEncryptionScheme
```

## Topics

### Creating an encryption scheme

init(rawValue: String)

Initialize an encryption scheme using a string.

### Encryption schemes

static let ECC_V2: PKEncryptionScheme

The elliptic curve cryptography (ECC) scheme.

static let RSA_V2: PKEncryptionScheme

The RSA v2 scheme.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Creating a request configuration

init?(encryptionScheme: PKEncryptionScheme)

Instantiates a new request configuration with the given encryption scheme.

