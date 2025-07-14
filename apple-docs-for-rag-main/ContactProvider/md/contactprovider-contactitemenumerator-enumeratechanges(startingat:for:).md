

- ContactProvider
- ContactItemEnumerator
-  enumerateChanges(startingAt:for:) 

Instance Method

# enumerateChanges(startingAt:for:)

Enumerates items changed since the last sync.

iOS 18.0+iPadOS 18.0+

``` source
func enumerateChanges(
    startingAt syncAnchor: ContactItemSyncAnchor,
    for observer: any ContactItemChangeObserver
) async
```

**Required**

## Parameters 

`syncAnchor`  

The sync anchor to enumerate changed items from.

`observer`  

The system observer that receives the change items and enumeration state.

## Discussion

The system calls `enumerateChanges(startingAt:for:)` for each batch of changed items to enumerate. After enumerating each batch of changed items, your implementation calls didFinishEnumeratingChanges(upTo:moreComing:) .

Your implementation can enumerate items in any order, but that order must be deterministic and resumable.

## See Also

### Enumerating item changes

struct ContactItemSyncAnchor

A snapshot point into enumerating changed contact items.

protocol ContactItemChangeObserver

A protocol that defines a system observer that receives a resumable enumeration of changed contact items.

