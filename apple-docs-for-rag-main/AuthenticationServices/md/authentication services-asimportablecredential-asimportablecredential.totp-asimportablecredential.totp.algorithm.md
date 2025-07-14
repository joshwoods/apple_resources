

- Authentication Services
- ASImportableCredential
- ASImportableCredential.TOTP
-  ASImportableCredential.TOTP.Algorithm 

Enumeration

# ASImportableCredential.TOTP.Algorithm

An enumeration of algorithm types that all importers are expected to support.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+visionOS 2.2+

``` source
enum Algorithm
```

## Topics

### Algorithms

case sha1

The SHA-1 algorithm.

case sha256

The SHA-256 algorithm.

case sha512

The SHA-512 algorithm.

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Accessing TOTP properties

var secret: Data

The secret associated with this generator.

var period: UInt16

The period, in seconds, used by the generator to refresh codes.

var digits: UInt16

The number of digits in the code used by the generator.

var username: String

The username associated with the generator.

var algorithm: ASImportableCredential.TOTP.Algorithm

The algorithm used by the generator.

var issuer: String?

The issuer of the generator, if any.

