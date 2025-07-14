

- Authentication Services
-  ASImportableAccount 

Structure

# ASImportableAccount

An account for use in importing and exporting credentials.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+visionOS 2.2+

``` source
struct ASImportableAccount
```

## Overview

This type is a representation of `Account` as defined in the Credential Exchange Format (CXF) specification. You can supply a JSON representation of a CXF `Account` to initialize an instance of this struct by using a JSONDecoder and calling decode(_:from:).

The account represents the user of the password manager app itself. You can export multiple accounts together by including them in an ASExportedCredentialData instance.

## Topics

### Creating an account

init(id: Data, userName: String, email: String, fullName: String?, collections: [ASImportableCollection], items: [ASImportableItem])

Creates an account instance from its required and optional properties.

### Accessing account properties

var id: Data

A unique identifier for the account.

var userName: String

The username associated with the account.

var email: String

The email address associated with this account.

var fullName: String?

The full name of the account owner, if provided.

var collections: [ASImportableCollection]

The collections stored in this account.

struct ASImportableCollection

A collection of items and subcollections for use in import and export.

var items: [ASImportableItem]

All items stored in the account.

struct ASImportableItem

An item for use in import and export.

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Accessing accounts

var accounts: [ASImportableAccount]

An array of importable accounts.

