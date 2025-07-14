

- Authentication Services
- ASImportableLinkedItem
-  init(item:account:) 

Initializer

# init(item:account:)

Creates a linked item from the identifiers of an item and an account.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+visionOS 2.2+

``` source
init(
    item: Data,
    account: Data? = nil
)
```

## Parameters 

`item`  

The id of the item linked by this `LinkedItem`.

`account`  

The id of the Account to which this `LinkedItem` belongs, if any. Defaults to `nil`.

