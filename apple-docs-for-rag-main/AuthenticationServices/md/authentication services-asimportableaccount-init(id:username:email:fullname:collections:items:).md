

- Authentication Services
- ASImportableAccount
-  init(id:userName:email:fullName:collections:items:) 

Initializer

# init(id:userName:email:fullName:collections:items:)

Creates an account instance from its required and optional properties.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+visionOS 2.2+

``` source
init(
    id: Data,
    userName: String,
    email: String,
    fullName: String? = nil,
    collections: [ASImportableCollection],
    items: [ASImportableItem]
)
```

## Parameters 

`id`  

A unique identifier for the account.

`userName`  

The username associated with the account.

`email`  

The email address associated with the account.

`fullName`  

The full name of the account owner, if provided.

`collections`  

An array of ASImportableCollection instances to store in the account.

`items`  

An array of ASImportableItem instances to store in the account.

