

- ContactProvider
- ContactItemChangeObserver
-  didFinishEnumeratingChanges(upTo:moreComing:) 

Instance Method

# didFinishEnumeratingChanges(upTo:moreComing:)

Marks a sync anchor of changed contact items as completed.

iOS 18.0+iPadOS 18.0+

``` source
func didFinishEnumeratingChanges(
    upTo syncAnchor: ContactItemSyncAnchor,
    moreComing: Bool
)
```

**Required**

## Parameters 

`syncAnchor`  

The `ContactItemSyncAnchor` where the next change enumeration should start from.

`moreComing`  

If `true`, the enumerator receives another call to enumerateChanges(startingAt:for:).

## Discussion

A change enumeration can resume in the future, continuing from this sync anchor. Calling this method saves the current batch of changed items to the system Contacts database.

## See Also

### Ending enumeration

struct ContactItemSyncAnchor

A snapshot point into enumerating changed contact items.

func didFinishEnumeratingChangesWithError(any Error)

Finishes the change enumeration with an error, indicating failure, to the observer.

**Required**

