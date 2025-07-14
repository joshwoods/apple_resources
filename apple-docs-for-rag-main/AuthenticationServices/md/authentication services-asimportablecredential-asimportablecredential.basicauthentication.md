

- Authentication Services
- ASImportableCredential
-  ASImportableCredential.BasicAuthentication 

Structure

# ASImportableCredential.BasicAuthentication

A type to represent a basic authentication password.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+visionOS 2.2+

``` source
struct BasicAuthentication
```

## Overview

This type is a representation of `BasicAuth` as defined in the Credential Exchange Format (CXF) specification.

## Topics

### Creating a basic authentication instance

init(urls: [String], username: ASImportableEditableField?, password: ASImportableEditableField?)

Creates a basic authentication password instance.

### Accessing authentication properties

var urls: [String]

The list of URLs for which to fill the password.

var username: ASImportableEditableField?

The username associated with the credential.

var password: ASImportableEditableField?

The password associated with the credential.

struct ASImportableEditableField

A field that someone can edit within a credential.

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

case passkey(ASImportableCredential.Passkey)

A passkey credential.

struct Passkey

A type to represent a passkey credential.

case totp(ASImportableCredential.TOTP)

A time-based one-time password (TOTP) credential.

struct TOTP

A type to represent a time-based one-time password generator (TOTP).

