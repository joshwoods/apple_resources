

- File Provider
-  NSFileProviderDomainDidChange 

Global Variable

# NSFileProviderDomainDidChange

A notification that posts when a file provider’s domain changes.

iOS 16.0+iPadOS 16.0+macOS 11.0+visionOS 1.0+

``` source
extern NSNotificationName const NSFileProviderDomainDidChange;
```

## Discussion

The system only posts this notification after the first call to getDomainsWithCompletionHandler(_:). After receiving this notification, call getDomainsWithCompletionHandler(_:) again to determine what the changes are.

## See Also

### Global variables

NSFileProviderMaterializedSetDidChange

A notification that the system posts when the set of materialized items changes for your file provider extension.

NSFileProviderPendingSetDidChange

A notification that the system posts when the set of pending items changes for your file provider extension.

