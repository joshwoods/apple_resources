

- Authentication Services
- ASImportableCredential
-  ASImportableCredential.TOTP 

Structure

# ASImportableCredential.TOTP

A type to represent a time-based one-time password generator (TOTP).

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+visionOS 2.2+

``` source
struct TOTP
```

## Overview

This type is a representation of `TOTP` as defined in the Credential Exchange Format (CXF) specification.

## Topics

### Creating a TOTP instance

init(secret: Data, period: UInt16, digits: UInt16, username: String, algorithm: ASImportableCredential.TOTP.Algorithm, issuer: String?)

Creates a time-based one-time password (TOTP) instance.

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

enum Algorithm

An enumeration of algorithm types that all importers are expected to support.

var issuer: String?

The issuer of the generator, if any.

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Login credential types

case basicAuthentication(ASImportableCredential.BasicAuthentication)

A password credential.

struct BasicAuthentication

A type to represent a basic authentication password.

case passkey(ASImportableCredential.Passkey)

A passkey credential.

struct Passkey

A type to represent a passkey credential.

case totp(ASImportableCredential.TOTP)

A time-based one-time password (TOTP) credential.

