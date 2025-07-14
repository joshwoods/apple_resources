

- Authentication Services
- ASImportableCredential
- ASImportableCredential.TOTP
-  algorithm 

Instance Property

# algorithm

The algorithm used by the generator.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+visionOS 2.2+

``` source
var algorithm: ASImportableCredential.TOTP.Algorithm
```

## Discussion

This value must be one of ASImportableCredential.TOTP.Algorithm.sha1, ASImportableCredential.TOTP.Algorithm.sha256, or ASImportableCredential.TOTP.Algorithm.sha512.

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

enum Algorithm

An enumeration of algorithm types that all importers are expected to support.

var issuer: String?

The issuer of the generator, if any.

