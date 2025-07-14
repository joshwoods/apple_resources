

- AppKit
- NSTextElementProvider
-  synchronizeToBackingStore(\_:) 

Instance Method

# synchronizeToBackingStore(\_:)

Synchronizes changes to the backing store.

macOS 12.0+

``` source
func synchronizeToBackingStore(_ completionHandler: (((any Error)?) -> Void)? = nil)
```

``` source
func synchronizeToBackingStore() async throws
```

**Required**

## Parameters 

`completionHandler`  

A completion handler to run upon successful completion, or to process an error upon failure.

## Discussion

If `completionHandler` is `nil`, performs the operation synchronously. The `completionHandler` gets passed `error` if the synchronization fails. It should block (or fails if synchronous) when there’s an active transaction.

