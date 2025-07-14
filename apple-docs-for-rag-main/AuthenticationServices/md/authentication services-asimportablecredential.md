

- Authentication Services
-  ASImportableCredential 

Enumeration

# ASImportableCredential

A credential for use in import and export.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+visionOS 2.2+

``` source
enum ASImportableCredential
```

## Overview

A credential represents a piece of secure information associated with an item. `ASImportableCredential` currently supports the following kinds of credentials:

- Password (`BasicAuthentication`)

- Passkey

- Time-based one-time password (TOTP)

- Note

- Credit card

This type is a representation of `Credential` as defined in the Credential Exchange Format (CXF) specification. You can supply a JSON representation of a CXF `Credential` to initialize an instance of this struct by using a JSONDecoder and calling decode(_:from:).

## Topics

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

struct TOTP

A type to represent a time-based one-time password generator (TOTP).

### Document credential types

case note(ASImportableCredential.Note)

A note credential.

struct Note

A piece of text used to store some information about an item.

### Identity credential types

case creditCard(ASImportableCredential.CreditCard)

A credit card credential.

struct CreditCard

A type to represent credit card information.

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Accessing item properties

var id: Data

A unique identifier for the item.

var created: Date

The item’s creation date and time.

var lastModified: Date

The item’s last modified date and time.

var type: ASImportableItem.ItemType

The type of the item.

enum ItemType

The type of an importable item.

var subtitle: String?

A subtitle or description of this item, if any.

var credentials: [ASImportableCredential]

The credentials associated with this item.

var tags: [String]

The user-defined tags associated with this item, if any.

