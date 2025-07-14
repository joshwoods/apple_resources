

- ContactProvider
- ContactItemChangeObserver
-  didFinishEnumeratingChangesWithError(\_:) 

Instance Method

# didFinishEnumeratingChangesWithError(\_:)

Finishes the change enumeration with an error, indicating failure, to the observer.

iOS 18.0+iPadOS 18.0+

``` source
func didFinishEnumeratingChangesWithError(_: any Error)
```

**Required**

## Discussion

Use `ContactProviderError.changeAnchorExpired` to restart the content enumeration.

## See Also

### Ending enumeration

func didFinishEnumeratingChanges(upTo: ContactItemSyncAnchor, moreComing: Bool)

Marks a sync anchor of changed contact items as completed.

**Required**

struct ContactItemSyncAnchor

A snapshot point into enumerating changed contact items.

