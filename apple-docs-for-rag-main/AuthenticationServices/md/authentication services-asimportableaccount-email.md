

- Authentication Services
- ASImportableAccount
-  email 

Instance Property

# email

The email address associated with this account.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+visionOS 2.2+

``` source
var email: String
```

## See Also

### Accessing account properties

var id: Data

A unique identifier for the account.

var userName: String

The username associated with the account.

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

