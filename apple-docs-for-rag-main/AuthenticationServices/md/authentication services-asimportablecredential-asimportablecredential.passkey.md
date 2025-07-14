

- Authentication Services
- ASImportableCredential
-  ASImportableCredential.Passkey 

Structure

# ASImportableCredential.Passkey

A type to represent a passkey credential.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+visionOS 2.2+

``` source
struct Passkey
```

## Overview

This type is a representation of `Passkey` as defined in the Credential Exchange Format (CXF) specification.

## Topics

### Creating a passkey instance

init(credentialID: Data, relyingPartyIdentifier: String, userName: String, userDisplayName: String, userHandle: Data, key: Data)

Creates a passkey instance.

### Accessing passkey properties

var credentialID: Data

The credential ID associated with this passkey.

var relyingPartyIdentifier: String

The relying party identifier associated with the passkey.

var userName: String

The username associated with the passkey.

var userDisplayName: String

The human-readable name associated with the passkey.

var userHandle: Data

The user handle associated with the passkey.

var key: Data

The private key associated with this passkey.

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

case totp(ASImportableCredential.TOTP)

A time-based one-time password (TOTP) credential.

struct TOTP

A type to represent a time-based one-time password generator (TOTP).

