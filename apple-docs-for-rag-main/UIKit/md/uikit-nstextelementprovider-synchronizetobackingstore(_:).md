

- UIKit
- NSTextElementProvider
-  synchronizeToBackingStore(\_:) 

Instance Method

# synchronizeToBackingStore(\_:)

Synchronizes changes to the backing store.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

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

