

- ContactProvider
- ContactItemEnumerating
-  enumerator(for:) 

Instance Method

# enumerator(for:)

Provide an enumerator for the contact items collection.

iOS 18.0+iPadOS 18.0+

``` source
func enumerator(for collection: ContactItem.Identifier) -> any ContactItemEnumerator
```

**Required**

## Parameters 

`collection`  

The collection to enumerate; defaults to rootContainer.

## Discussion

The collection represents all contacts for the domain (`ContactItem.Identifier.rootContainer`).

## See Also

### Providing an enumeration

struct Identifier

The app’s identifier for an item in the contact database.

protocol ContactItemEnumerator

A protocol to provide enumerations of all contact items and changed contact items.

