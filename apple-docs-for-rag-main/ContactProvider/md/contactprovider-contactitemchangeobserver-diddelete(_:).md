

- ContactProvider
- ContactItemChangeObserver
-  didDelete(\_:) 

Instance Method

# didDelete(\_:)

Provides an array of deleted contact item identifiers to the observer.

iOS 18.0+iPadOS 18.0+

``` source
func didDelete(_ identifiers: [ContactItem.Identifier])
```

**Required**

## Parameters 

`identifiers`  

The identifiers of the deleted items.

## Discussion

You can call this method multiple times to fulfill the suggestedBatchSize.

## See Also

### Providing change data

func didUpdate([ContactItem])

Provides an array of new and updated contact items to the observer.

**Required**

enum ContactItem

An item in the contact database.

struct Identifier

The app’s identifier for an item in the contact database.

