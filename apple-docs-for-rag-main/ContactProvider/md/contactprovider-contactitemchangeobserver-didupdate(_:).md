

- ContactProvider
- ContactItemChangeObserver
-  didUpdate(\_:) 

Instance Method

# didUpdate(\_:)

Provides an array of new and updated contact items to the observer.

iOS 18.0+iPadOS 18.0+

``` source
func didUpdate(_ items: [ContactItem])
```

**Required**

## Parameters 

`items`  

The new and updated items.

## Discussion

You can call this method multiple times to fulfill the suggestedBatchSize. The observer creates the new contact items and updates the existing contact items with their new values.

## See Also

### Providing change data

enum ContactItem

An item in the contact database.

func didDelete([ContactItem.Identifier])

Provides an array of deleted contact item identifiers to the observer.

**Required**

struct Identifier

The app’s identifier for an item in the contact database.

